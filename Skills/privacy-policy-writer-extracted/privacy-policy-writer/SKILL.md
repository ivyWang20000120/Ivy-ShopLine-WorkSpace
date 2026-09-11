---
name: privacy-policy-writer
description: 为 Shopline 应用市场插件撰写、生成或改写隐私政策（Privacy Policy）文档。当用户提到"写隐私政策"、"帮我生成一份隐私政策"、"仿照这个隐私政策写一份"、"给 XX 插件写隐私政策"、"privacy policy"、"隐私协议"、"数据政策"等关键词时，主动使用本 skill。即使用户只描述了插件的功能，也应先套用本 skill 的结构模板再输出，不要临时自创格式。适用于 Shopline 平台各类插件（电商合规类、ERP同步类、营销类、支付类等），只需替换变量占位符即可快速生成符合 Shopline 应用市场要求的完整隐私政策。
---

# Privacy Policy Writer — Shopline 插件隐私政策生成 Skill

## 概述

本 skill 用于为 Shopline 应用市场插件快速生成标准化、合规的隐私政策文档。模板基于 Silk 公司已发布的隐私政策（Lingxing ERP Inventory Sync、电子销售合同插件等）提炼而成，结构符合 Shopline 应用市场要求，同时兼顾 GDPR、土耳其 KVKK 等常见合规场景。

**输出格式**：Markdown 文件（.md），可直接用于 Shopline 应用市场上架或公司官网发布。

---

## 使用前：收集必要信息

在生成隐私政策前，需确认以下信息（未提供的字段使用默认值或占位符）：

| 变量 | 说明 | 默认值 |
|------|------|--------|
| `{{APP_NAME}}` | 插件完整名称 | 必填 |
| `{{OPERATOR_EN}}` | 运营主体英文名 | Chengdu Silk Software Co., Ltd. |
| `{{OPERATOR_CN}}` | 运营主体中文名 | 成都思而科软件有限公司 |
| `{{LAST_UPDATED}}` | 最后更新日期 | 当天日期 |
| `{{EFFECTIVE_DATE}}` | 生效日期 | 当天日期 |
| `{{YEAR}}` | 版权年份 | 当前年份 |
| `{{SUPPORT_EMAIL}}` | 客服邮箱 | apps@silksoftware.com |
| `{{DATA_EMAIL}}` | 数据删除邮箱 | apps@silksoftware.com |
| `{{WEBSITE}}` | 官网地址 | https://www.silksoftware.com.cn/ |
| `{{ADDRESS}}` | 公司地址 | 成都市武侯区天府软件园E2-1栋3楼 |

如果用户已提供插件功能描述，从中提取：
- 插件的**核心能力**（3~5 条 bullet，写入第 0 节 Welcome 段落）
- 插件**收集的特殊数据类型**（写入 Section 3）
- 插件的**特殊数据保留要求**（如有法规要求，写入 Section 6）
- 插件**依赖的第三方服务**（写入 Section 8 / Section 14）

---

## 生成流程

### Step 1：读取模板
读取 `assets/电子销售合同插件_隐私政策_模板.md` 作为基础结构。

### Step 2：替换变量
将所有 `{{变量名}}` 替换为用户提供的实际值或默认值。

### Step 3：按插件类型定制内容

根据插件功能类型，重点调整以下章节：

#### 🔵 电商合规类（如电子合同、消费者知情同意）
- Section 3.1：增加「消费者结算页数据」子项（买方信息、商品信息、金额等）
- Section 3.1：增加「生成的合同数据」子项（PDF内容、合同ID、署名等）
- Section 4.1：重点描述合同生成、强制同意、存储与订单绑定流程
- Section 5：Legal Bases 增加「Legal obligation（土耳其远程销售法）」
- **保留 Section 6（合同数据保留与不可篡改性）**，这是合规类插件专属章节

#### 🟡 ERP / 库存同步类
- Section 3.1：增加「商品与目录数据」「订单与履约数据」「仓库配置数据」
- Section 4.1：描述库存轮询、退货处理、幂等性控制等
- **删除 Section 6**（无特殊保留要求时）
- Section 14：列出依赖的 ERP 系统（如领星 ERP）

#### 🟢 营销 / 邮件 / 推荐类
- Section 3.1：增加「营销偏好与行为数据」
- Section 4.1：描述邮件发送、用户分群、A/B 测试等
- Section 5：Legal Bases 增加「Consent（营销类必须）」
- **删除 Section 6**

#### 🔴 支付 / 金融类
- Section 3.1：增加「支付方式信息（不含完整卡号/CVV）」
- Section 3.4：明确说明不存储完整支付卡信息
- Section 11：加强安全措施描述（PCI DSS 等）

### Step 4：质量检查

生成后确认以下各项：
- [ ] 所有 `{{占位符}}` 均已替换
- [ ] 插件核心能力描述与用户需求一致
- [ ] 数据收集条目与插件实际功能匹配（无多收、无漏收）
- [ ] 第三方服务（Shopline、ERP、云存储等）在 Section 8 / 14 中均已提及
- [ ] 特殊合规要求（如土耳其法规）已在 Section 5 / 6 体现
- [ ] 联系方式信息完整

### Step 5：输出

将最终隐私政策保存为 `.md` 文件并通过 `present_files` 提供下载。同时在对话中简要说明：
- 哪些章节做了定制化修改
- 哪些占位符需要用户后续确认填写

---

## 章节结构说明

标准隐私政策共 17 个章节，结构如下：

```
0. Welcome / 产品功能简介（非编号，写在标题下方）
1. Scope — 适用范围
2. Our Role — 数据处理角色
3. Information We Collect — 信息收集
   3.1 Shopline 授权获取
   3.2 用户主动提供
   3.3 设备与使用信息
   3.4 一般不收集的信息
4. How We Use Information — 使用目的
   4.1 核心功能（按插件类型定制）
   4.2 安全与风控
   4.3 客户支持与产品改进
   4.4 法律与合规
5. Legal Bases — 法律依据（Contract / Legitimate interests / Consent / Legal obligation）
6. 特殊数据保留条款（仅合规类插件保留此章节）
7. Cookies and Similar Technologies
8. How We Share Information — 数据共享
9. Data Retention — 数据保留
10. International Transfers — 跨境传输
11. Security — 安全措施
12. Your Rights — 用户权利
13. Uninstall and Deletion — 卸载与删除
14. Third-Party Sites — 第三方服务
15. Children's Privacy — 儿童隐私
16. Changes to This Policy — 政策变更
17. Contact Us — 联系方式
```

> **注**：合规类插件（如电子合同）在 Section 5 之后插入专属的 Section 6（合同数据保留与不可篡改性），原 Section 6 起顺延编号。非合规类插件无此章节，编号保持 5→6（Cookies）连续。

---

## 参考资产

- `assets/电子销售合同插件_隐私政策_模板.md`：电子销售合同插件完整隐私政策（合规类参考范本）

如需添加其他插件类型的范本，将对应 `.md` 文件放入 `assets/` 目录，并在本 SKILL.md 的「参考资产」章节补充说明。

---

## 快速示例

用户输入：
> "帮我给一个 Shopline 积分营销插件写隐私政策，插件功能是：消费者下单后自动发放积分，积分可用于下次购物抵扣。"

Claude 应当：
1. 识别为「营销类」插件
2. 从功能描述提取：自动积分发放、积分抵扣购物
3. 套用模板，选择营销类定制路径
4. 收集信息：APP_NAME（积分营销插件名称）、依赖的第三方积分系统（如有）
5. 输出完整隐私政策 `.md` 文件
