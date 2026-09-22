# 明汇企业套件

**Ming Enterprise Suite** 是面向企业业务的多项目集合，统一承载管理后台、基础设施以及 OA、ERP、CRM、MES、WMS、FMS、PMS、HRM、AI、IoT、IM 等业务模块。

- 后端仓库：<https://github.com/NicolasMing/ming-enterprise-suite>
- 前端仓库：<https://github.com/NicolasMing/ming-enterprise-suite-ui>
- 主前端目录：`yudao-ui/yudao-ui-admin-vue3`

## 项目范围

- 后端共有 46 个 Maven 项目描述文件；当前 Reactor 启用 21 个项目（包含根项目）。
- 前端目录共有 5 个项目，其中 Vue3 管理后台为完整源码，其余 4 个暂为可选前端说明目录。
- Vue3 前端清单声明 105 个直接依赖，锁文件已与清单对齐。

## 本地启动

后端需要 JDK 25、Maven、MySQL 与 Redis，入口为 `yudao-server`。前端需要 Node.js 20.19+ 与 pnpm 10：

```bash
cd yudao-ui/yudao-ui-admin-vue3
pnpm install --frozen-lockfile
pnpm dev
```

## 兼容与上游

为保证兼容性，当前阶段保留 `cn.iocoder.yudao` Java 包名、`yudao.*` 配置键、Maven 坐标及数据库技术标识。界面名称、仓库地址和运行时默认品牌统一为“明汇企业套件”。

本项目基于 [ruoyi-vue-pro](https://github.com/YunaiV/ruoyi-vue-pro) 与 [yudao-ui-admin-vue3](https://github.com/yudaocode/yudao-ui-admin-vue3) 持续维护，保留原项目许可证、作者署名和第三方归属。来源说明见 [docs/UPSTREAM_README.md](docs/UPSTREAM_README.md)。
