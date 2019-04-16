# Framework 1 Checklist #
---
**Issues**
- Goes to "password" page and not "index"
- User update haven't implemented
- User remove haven't implemented
- Employee update error [session cookie/authcookie error]
- Company create suddenly breaks
---
## User Management ##
- add "Logout" to navbar
- hash password
- create User
- show User detail
- update User
- include users: [Kevin/Barnes, admin/Admin, your Firstname/Lastname] 
---
#### Check Admin Role ####
- add following to [ controllers / main.cfc  ~  processLogin() ] to check admin role
- ![checkAdmin](https://user-images.githubusercontent.com/46738881/56229531-bce76c00-603f-11e9-9df1-d2510f14e0ba.PNG)
- add following to userService.cfc
- ![checkAdmin2](https://user-images.githubusercontent.com/46738881/56230599-3f712b00-6042-11e9-9d3d-ae9e97bbc0b9.PNG)
---  
#### Page that got used/implemented ####
- *Controller / userManagement*
- *Model / domain / admin.cfc*
- *Model / domain / user.cfc*
- *Model / gateway / userGateway.cfc*
- *Controller / service / userService.cfc*
- *Views / userManagement / userCreate.cfm* 
- *Views / userManagement / userDetail.cfm* 
- *Views / userManagement / userList.cfm*  
- *Views / userManagement / userUpdate.cfm* 
---  
## Employee Management ##
- list employees 
- show employee details
- create new employee
- remove employee
---  
#### Page that got used/implemented ####
- *Controller / employeeManagement*
- *Model / domain / employee.cfc*
- *Controller / service / employeeService.cfc*
- *Views / employeeManagement / employeerCreate.cfm* 
- *Views / employeeManagement / employeeDetail.cfm* 
- *Views / employeeManagement / employeeList.cfm*   
- *Views / employeeManagement / employeeUpdate.cfm*
---    
## Company Management ##
- list only active companies
- show only employee(s) that works for the particular company
- show company detail [had to make a button instead of clickable row due to modal]
- in modal, user can update employee information, href leads back to update page
- 
- *company updated [but gave error]*
---
#### Soft Delete ####
  - implement "Soft Delete" instead of delete by setting a flag (isRemoved)
  - ![softDelete](https://user-images.githubusercontent.com/46738881/56235006-181f5b80-604c-11e9-8c63-588ccba939e5.PNG)
---
#### Page that got used/implemented ####
- *Controller / companyManagement*
- *Model / domain / company.cfc*
- *Controller / service / companyService.cfc*
- *Views / companyManagement / companyCreate.cfm* 
- *Views / companyManagement / companyDetail.cfm* 
- *Views / companyManagement / companyList.cfm*   
- *Views / companyManagement / companyUpdate.cfm*
---
#### Routes used/implemented ####
![routes](https://user-images.githubusercontent.com/46738881/56236365-0d19fa80-604f-11e9-875b-7a9e6f0e202c.PNG)
