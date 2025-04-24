# 📦 SICAP Web

## 🧭 Overview
**SICAP Web** is a performance-focused enterprise application designed for executive leadership to monitor project execution, contract compliance, and operational KPIs across a construction and engineering organization. Originally a Windows Forms application hosted internally on IIS, the system is purpose-built for high-level decision-making, surfacing real-time analytics, contract lifecycle metrics, and vendor estimation insights in a centralized, secure interface.

> This tool plays a **critical role in weekly leadership reviews**, enabling data-driven decisions and exception management across millions in active projects.

![Screenshot](./assets/sicap-home.png) <!-- Replace with your image path -->

## 💡 Idea & Concept
The initiative originated from a strategic need to:
- Provide a **cross-platform, visually intuitive interface** for managers and directors—especially those on macOS who were previously blocked from accessing internal systems.
- Shift the focus from raw operations to **executive-level KPIs**, highlighting contract risk, overdue projects, and payment bottlenecks.
- Offer drill-down capabilities from macro trends (on-time project ratios) to micro-levels (performance per engineer or vendor).

The project served as a modernization of a legacy desktop system, bridging classic infrastructure with modern data visualization and dashboard patterns.

## ✨ Features & Functionality
- 🔐 **Authentication Layer**: Secure login with role-based access
- 🏠 **Executive Dashboard** (Windows 10 UX):
  - KPI-driven modules: Active Projects, Vendor Applications, Contract Additions, Team Capacity, and more
  - Traffic light indicators (RAG system) based on configurable thresholds
- 📊 **Interactive Analytics**:
  - Drillable bar charts: Project timelines, monthly performance
  - Summary tables with trendlines, thresholds, and real vs. target metrics
  - Dynamic links to sub-reports per department, area, and engineer
- 📁 **Data Query Engine**:
  - Advanced filters for contracts, estimations, personal/vendor contracts, and extension requests
- 📤 **Export & Reporting Tools**:
  - Excel export of filtered views
  - Planned Crystal Reports integration for PDF generation
- 👤 **User Profile Management**

## ⚙️ Tech Stack
- **Frontend**: HTML, CSS, JavaScript, jQuery  
- **Backend**: Visual Basic .NET, SQL Server  
- **Architecture**: Windows Forms Application hosted via IIS (intranet-based)  
- **Data Pipeline**: Summary tables via automated SQL jobs (ETL-style)  
- **Reporting**: Planned Crystal Reports + Excel export

## 🏗 Architecture & Design
- **Modular UI with block navigation**, modeled after Windows 10 UX
- **Pre-aggregated data layer** powered by scheduled Windows services for **performance at scale**
- **Navigation flow**: Dashboard → KPIs → Summary Tables → Drilldown Reports → Detailed Contract View
- **Responsive breakdown logic** to explore data hierarchically: from company-level down to the individual engineer

## 🚀 Installation & Setup
- **Deployment**: Hosted on internal Windows IIS servers
- **Data Source**: SQL Server with ETL-style background jobs for data consolidation
- **Access**: Internal-only; authenticated users via company credentials

> **Note:** Setup and deployments are handled by the internal IT department.

## 🧑‍💻 My Role & Contributions
As a core contributor during my tenure, I:
- 🗄 Engineered high-performance SQL procedures for pre-aggregated KPIs and reporting views  
- 🧱 Designed and built key UI components using WinForms and jQuery for interactive dashboards  
- 🎨 Led the UX workstream for block-based layout and RAG-style visualization  
- 🔁 Wrote reusable stored procedures and optimized cross-table joins for scalable performance  
- 🧪 Owned end-to-end QA testing including boundary cases and report validation  
- 🤝 Collaborated daily with a senior developer to align business needs with technical feasibility

## 🧗 Challenges & Learnings
- Navigated a steep learning curve with **legacy WinForms UI and Visual Basic .NET**, while introducing modern best practices
- Built a **data summary strategy** using SQL ETL-style jobs to handle scale and latency issues
- Balanced the needs of executive stakeholders (macOS compatibility, summary focus) with legacy system constraints
- Gained firsthand experience in **enterprise data governance, stakeholder communications, and multi-tier architecture**

## 📈 Future Enhancements
- ✅ Migrate the application to a Web-first architecture using ASP.NET MVC or .NET Core  
- 📱 Introduce responsive design for mobile access  
- 🧾 Implement PDF reporting (Crystal Reports) and scheduled email digests  
- 🔍 Build a dynamic search and tagging system for project tracking and alerts  

## 🤝 Contributing
This application is used internally across the organization by management. Future iterations and new modules are planned and maintained by the IT & Software Engineering team.

## 🪪 License
⚠️ License Notice  
This repository was originally published under the MIT License.  
As of April 22, 2025, the license has been changed to **CC BY-NC-ND 4.0**.  
See the LICENSE file for details.

## 🔗 Additional Resources
- **Documentation:** Available via company SharePoint  
- **Related Systems:** SICAP Desktop (Legacy), Vendor Portal, Budget Review Tool  
- **Live Demo Link:** Restricted (internal access only)