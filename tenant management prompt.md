

> **GOAL: Designing a "Tenant Management" (租户管理) page for an Enterprise Procurement Platform Management System (运营后台).**
> 
> **Visual Styles (Strict Follow)**:
> 
> - Primary Brand Color: `#0A62CA`.
>     
> - Interaction Colors: Hover `#4080FF`, Pressed `#0958B6`, Disabled `#94BFFF`.
>     
> - Typography: Base font size 14px. Headings use Medium weight.
>     
> - Text Hierarchy Colors: Primary `#1D2129`, Secondary `#4E5969`, Muted `#86909C`.
>     
> - Style: Modern, clean, professional B-side interface.
> 
> Chinese body & headings:** Use `CN` font family (system Chinese font or Source Han Sans CN / PingFang SC)
> 
> English body & headings:** Use a clean geometric sans-serif — `EN` font (Inter or similar enterprise-grade font is acceptable here given the institutional context)
>     

# Tenant Management List 

> 1. **Header**: Title "租户管理".
>     
> 2. **Search Filter Bar**: Include inputs for "租户名称" (Tenant Name), "租户代码" (Social Credit Code), "租户类型" (Dropdown: 招标人/采购人), "联系人", and a Date Range Picker for "入驻时间". Include "查询" (Search) and "重置" (Reset) buttons.
>     
> 3. **Action Bar**: A button for "批量导入" (Bulk Import) with an icon.
>     
> 4. **Data Table**:
>     
>     - Columns: 租户名称, 租户代码, 租户类型, 联系人, 联系电话, 入驻时间, 操作 (Actions).
>         
>     - Action Column: Display text links for "编辑" (Edit), "设置权限" (Permissions), "关联收费规则" (Fees), "运营用户" (Users), "组织架构" (Org), and a red "删除" (Delete) button.
>         
> 5. **Pagination**: Standard pagination at the bottom right.
>     
> 
> **Output Requirement**: Generate a high-fidelity web UI mockup. Ensure all labels and data entries are in **Simplified Chinese**.

---
# Edit Tenant Drawer 

> **Context**: A side drawer (抽屉) for "编辑租户" (Edit Tenant).
> 
> **Layout**:
> 
> - Divided into sections: "基本信息" (Basic Info) and "网页配置" (Web Config).
>     
> - **Form Fields**: Tenant Name, Type (Multi-select), Social Credit Code, Contact Person, Phone, etc.
>     
> - **Upload Area**: Specific upload slots for "企业管理后台Logo", "采购系统Logo", and "监督系统Logo" (Size hint: 457x28).
>     
> - **Footer**: "取消" (Cancel) and "提交" (Submit) buttons using primary brand colors.
>     
>     **Requirement**: Keep all UI text in Chinese. Follow the `#0A62CA` color scheme.
>     


# Permission Settings

- **Header**: Title "个性化权限配置".
    
- **Form Structure**:
    
    - **门户网站**: Radio group (使用 / 不使用).
        
    - **接口平台登录**: Switch (是 / 否).
        
    - **平台使用费**: Switch (收取 / 不收取).
        
    - **自查报告**: Radio group (使用 / 不使用).
        
    - **允许招标代理**: Multi-select link/button. Clicking shows a selection list of "代理机构名称" and "企业代码".
        
- **Footer**: "返回" and "确认配置" buttons.


# Fee Rules 

> 
> - **Header**: Title "租户收费标准维护".
>     
> - **Description**: A tip text "请选择该租户执行的收费规则模板".
>     
> - **Fields**:
>     
>     - **招标规则名称**: Searchable Select (Options pulled from 平台使用费规则).
>         
>     - **非招规则名称**: Searchable Select (Options pulled from 平台使用费规则).
>         
> - **Special Display**: A preview area showing the "多中标人收费占比" logic if a rule is selected.
>     
> - **Footer**: "提交".
>


# Admin User list 


> **Context**: Design a wide Modal for "运营用户管理"
> 
> - **Header**: Title "关联运营管理员列表".
>     
> - **Search Bar**: "姓名/用户名" search input and "搜索" button.
>     
> - **Data Table**:
>     
>     - **Columns**: 姓名, 用户名, 已分配角色 (e.g., 平台运营, 信息审核员), 账号状态.
>         
>     - **Status Column**: Use a Toggle/Switch for "有效/无效".
>         
> - **Actions**: "重置密码" and "禁用".
>     
> - **Footer**: "关闭".

### The Total Menu Architecture

> **Generate a vertical sidebar navigation menu for the "Procurement Operations Backend" (运营后台). **CRITICAL:** All menu titles must be in **Simplified Chinese**.
> 
> 
> - **Background**: High-contrast dark or clean white theme.
>     
> - **Active State**: Highlight the selected menu item using Brand Color `#0A62CA` with a light blue background fill (Brand1-2: `#BEDAFF`).
>     
> - **Typography**: 14px base font, Medium weight for top-level menus.
>     
> 
> **Menu Structure & Icons**
> 
> 1. **租户管理 (Tenant Management)**: Icon - Group/Building.
>     
>     - Includes: 租户配置, 组织架构, 默认角色配置.
>         
> 2. **权限管理 (Permission Management)**: Icon - Lock/Shield.
>     
>     - Includes: 运营用户管理, 运营角色权限.
>         
> 3. **企业管理 (Enterprise Management)**: Icon - Bank/Verified.
>     
>     - Includes: 用户查询, 企业注册审批, 信息变更审核, 账号申诉审核.
>         
> 4. **供应商管理 (Supplier Management)**: Icon - Truck/UserCheck.
>     
>     - Includes: 主数据维护, 信用审计, 协同供应商库.
>         
> 5. **采购管理 (Procurement Supervision)**: Icon - BarChart/Monitor.
>     
>     - Includes: 采购制度复核, 立项合规复核, 交易监控.
>         
> 6. **运营管理 (Platform Operations)**: Icon - Tool/Notification.
>     
>     - Includes: 门户内容管理, 运营维保工具, 接口平台管理.
>         
> 7. **全局日志审计 (Audit Logs)**: Icon - FileSearch.
>     
>     - Includes: 跨系统操作日志.
>         
> 8. **系统配置 (System Config)**: Icon - Settings.
>     
>     - Includes: 子系统及菜单维护.
>