# G5/G9 产品修改记录

- 产品编号：$(@{number=93; product_id=JLZ-EDU-SK-075; chinese_name=教学服务标准核查; english_name=Teaching Service Standard Checker; repository_name=edu-teaching-service-standard-checker; repository_url=https://github.com/jinlize-tech/edu-teaching-service-standard-checker; product_type=Skill; category_code=08; category=08 校区标准化与多校区管理中心; description=教学服务标准核查。; target_users=System.Object[]; core_input=课程标准、教学流程、课堂/作业/反馈证据、教师行为和检查标准; main_output=标准核查表、证据缺口、偏差分级、整改项和复核标准; product_risk=用单一课堂样本评价教师或泄露学生信息; dedup_label=存在部分功能交叉; dedup_note=与课堂观察量表区别：本产品核查教学服务标准体系；后者只生成一节课观察工具。; development_status=Planned / 待研发; license=Apache-2.0; spec_version=1.0.0; workbuddy_status=PLANNED_FOR_WORKBUDDY}.product_id)
- 产品名称：教学服务标准核查
- 基线：EDUCATION_BASELINE_V1.0.0
- 基线提交：$BaselineCommit
- 原版本：1.0.0
- 新版本：1.0.1

## 本次修改

1. 强化产品专属执行流程、输入核对和输出验收规则。
2. 新增 scripts/validate_input.js，实际检查必填字段、冲突、未确认数据和敏感信息。
3. 新增正常、缺失、冲突、敏感信息和非法JSON场景输入。
4. 测试升级为 T1–T7 分层并保存逐项检查结果。
5. 安装包加入 Apache-2.0 LICENSE 和 THIRD_PARTY_NOTICES.md。
6. 安装包升级为 1.0.1，加入许可证、第三方声明和输入校验脚本，保留 1.0.0 ZIP。
7. 按本产品冻结规格补充专属处理规则、输入到成果的核对矩阵和去重边界。

## 产品专属增强

- 核心任务：教学服务标准核查。
- 主要风险：用单一课堂样本评价教师或泄露学生信息
- 去重边界：与课堂观察量表区别：本产品核查教学服务标准体系；后者只生成一节课观察工具。

- 先明确标准版本、适用校区、检查范围、证据来源和例外条件。
- 按流程节点核对责任人、输入、完成标准、输出和升级机制。
- 区分现状证据、标准要求、差距、影响、整改动作和复验标准。
- 不代替机构作出处罚、人事、财务或行政批准决定。

## 运行边界

- 本地模型行为：NOT_RUNTIME_VERIFIED
- WorkBuddy平台验证：WORKBUDDY_VALIDATION_NOT_IN_SCOPE
- 本轮不执行上传、安装、审核或正式发布。
