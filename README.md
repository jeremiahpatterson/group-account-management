<p align="center">
<img src="https://i.imgur.com/qxo7Joc.jpeg" alt="Traffic Examination"/>
</p>

<h1>Group Policy and Account Management </h1>
In this tutorial, we will configure the lockout under Group Policy Management. We will also demonstrate account enabling and disabling.  <br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Active Directory


<h2>Operating Systems Used </h2>

- Windows 10 Enterprise, version 22H2 - x64 Gen2

<h2>High-Level Steps for Group Policy and Account Management</h2>

* Step 1 - On the Domain Controller, open the Group Policy Management Console, navigate to the correct domain, then right-click on Default Domain Policy to edit.
* Step 2 - Navigate to Account Lockout Policy > Define this policy setting and configure it as desired.    
* Step 3 - Verify the group policy.
  
<h2>Account Enabling</h2>

- Step 1 - Unlock the account.
- Step 2 - Verify account is accessible
- End Task


<h2>Actions and Observations</h2>

<p>
<img src="https://i.imgur.com/140Wk3T.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Click on Start, then navigate to Windows Administrative Tools > scroll down, and click on Group Policy Management. Select the correct domain, then right-click on Default Domain Policy to edit.

</p>
<br />

<p>
<img src="https://i.imgur.com/yzlATNV.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Click on Computer Configuration> Policies > Windows Settings > Security Settings > Account Lockout Policy. Within the Account Lockout Policy, set the desired durations.
</p>
<br />

<p>
<img src="https://i.imgur.com/VyNhkXv.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
On the User account, test the new policy by using the wrong password more times than your set limit to trigger a lockout. If you received a lockout message, you have configured the Group Policy successfully.
</p>
<br />

<p>
<img src="https://i.imgur.com/CKq1RHN.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
To unlock the account within Active Directory Users and Computers, locate the User within the proper folder, right-click on it, and select Properties > Account. Check the Unlock Account box, set the desired Account Password Options. Click Apply, then OK. 
</p>
<br />

<p>
<img src="https://i.imgur.com/6nN4QY7.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Verify that the User can now log in.
</p>
<br />
