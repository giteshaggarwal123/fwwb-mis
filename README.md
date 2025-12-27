# FWWB India - Integrated Management System Wireframes

## Overview
Complete, fully functional wireframes for FWWB (Friends of Women's World Banking) India's integrated management system covering Program Management, HRMS, and Administration modules.

## Features

### Program Management
- **Activities Management**: Track project activities with budget allocation, progress monitoring, and team assignments
- **Budget Management**: Project-wise budget tracking with utilization monitoring and alerts
- **Expenses & Bill Settlement**: Bill upload, verification, approval workflow with activity linkage
- **Monitoring & Data Collection**: Field data entry with offline/online support, GPS tagging, photo uploads, LFA indicator tracking
- **Reports & Dashboards**: Project-wise and donor-wise reporting with Excel/Word export

### HRMS (Human Resource Management System)
- **Recruitment**: Job posting, application tracking, shortlisting, and candidate management
- **Employee Management**: Complete employee lifecycle from onboarding to exit
- **Attendance Management**: GPS-based mobile attendance and biometric integration
- **Leave Management**: Leave application, approval workflow, and balance tracking
- **Performance Management**: KPI setting, goal tracking, 360-degree reviews, IDP creation
- **Payroll**: Salary processing with statutory compliance (PF, ESIC, TDS, PT)
- **Employee Self Service (ESS)**: Payslip download, leave application, profile updates
- **Exit Management**: Resignation processing, exit interviews, clearance certificates

### Administration
- **Asset Management**: IT and Non-IT asset tracking with warranty monitoring
- **Insurance Management**: Medical, Group Accident, Vehicle, Fire & Safety, D&O policies with renewal alerts
- **Travel Booking**: Multi-mode travel request and approval system
- **Stationery Management**: Request, approval, and stock management
- **Admin Expenses**: Expense submission and tracking

## Role-Based Access Control

The system implements role-based access with 4 user types:

1. **Management**: Full access to all modules
2. **Program Team**: Access to Program Management modules, attendance, leave, and ESS
3. **HR Team**: Access to all HRMS modules
4. **Admin Team**: Access to Administration modules, attendance, leave, and ESS

## Design & Branding

- **Colors**:
  - Primary: #2E3192 (Navy Blue)
  - Secondary: #1BADE3 (Cyan)
- **Typography**: System fonts (-apple-system, BlinkMacSystemFont, 'Segoe UI', Arial)
- **Responsive**: Mobile-friendly design
- **Professional**: Clean, modern UI aligned with FWWB branding guidelines

## Demo Credentials

### Login Information
Select a user type on the login screen and credentials will auto-populate:

- **Management**: admin / demo123
- **Program Team**: program.user / demo123
- **HR Team**: hr.user / demo123
- **Admin Team**: admin.user / demo123

## Technology Stack

- Pure HTML5, CSS3, and JavaScript
- No external dependencies
- Fully self-contained single-page application
- Dynamic screen generation
- GPS geolocation integration

## Local Testing

Simply open `index.html` in any modern web browser:

```bash
# Windows
start chrome index.html

# Mac
open index.html

# Linux
xdg-open index.html
```

## Deployment to Firebase

### Prerequisites
1. Install Node.js and npm
2. Install Firebase CLI:
   ```bash
   npm install -g firebase-tools
   ```

### Deployment Steps

1. **Login to Firebase**:
   ```bash
   firebase login
   ```

2. **Initialize Firebase Project** (if not already done):
   ```bash
   firebase init hosting
   ```
   - Select "Use an existing project" or "Create a new project"
   - Set public directory to: `.` (current directory)
   - Configure as single-page app: Yes
   - Don't overwrite index.html

3. **Deploy**:
   ```bash
   firebase deploy
   ```

4. **Access** your deployed site at:
   ```
   https://your-project-id.web.app
   ```

## Deployment to Vercel

1. **Install Vercel CLI**:
   ```bash
   npm install -g vercel
   ```

2. **Deploy**:
   ```bash
   vercel
   ```

3. **Follow prompts** to link/create project

## Project Structure

```
fwwb-wireframes-project/
│
├── index.html          # Main wireframes file
├── firebase.json       # Firebase hosting configuration
├── README.md          # This file
└── .git/              # Git repository
```

## Next Steps for Production

This is a wireframe/prototype. For production implementation:

1. **Backend Development**:
   - Node.js/Express or Python/Django REST API
   - PostgreSQL/MySQL database
   - Authentication & authorization (JWT)
   - File storage (AWS S3/Google Cloud Storage)

2. **Frontend Framework**:
   - React.js or Vue.js
   - State management (Redux/Vuex)
   - Component library (Material-UI/Ant Design)

3. **Mobile App**:
   - React Native or Flutter
   - GPS attendance integration
   - Offline data sync

4. **Integrations**:
   - Payment gateways
   - SMS/Email notifications
   - Biometric attendance devices
   - Accounting software (Tally/QuickBooks)
   - Power BI/Tableau for analytics

5. **Security**:
   - HTTPS/SSL
   - RBAC implementation
   - Data encryption
   - Audit logs
   - GDPR compliance

6. **DevOps**:
   - CI/CD pipeline
   - Automated testing
   - Monitoring & logging
   - Backup & disaster recovery

## Support & Contact

For questions or support:
- Email: palak.patel@fwwbindia.org
- Website: https://www.fwwbindia.org
- Office: 101, Sakar-I, Opp. Gandhigram Railway Station, Ashram Road, Ahmedabad 380 009, Gujarat, India
- Phone: +91-79-26580119

## License

© 2024 FWWB India. All rights reserved.

---

**Generated with Claude Code** - https://claude.com/claude-code
