# FORCED AUTHENTICATION

## Introduction
In this letsDefend Scenario an alert was triggered due to multipe post requests to the following URL: http://test-frontend.letsdefend.io/accounts/login

<br>
The Time range of these login attempts was 2:04 - 2:15pm.

<br>

## Per usual I looked up the reputation of the Source IP Address: 120.48.36.175
<br>

## Virus total shows that this is a Chinese IP that has been known for Brute Force attacks 
<img width="1898" height="926" alt="Suspicious Source IP" src="https://github.com/user-attachments/assets/fd00e7b9-e22f-4fa5-8dd3-2be8d13e920e" />
<br>

## The Screenshots below show the multiple login attempts with different username and password attempts that resemble a classic dictionary table attack.

<br>
  <img width="904" height="495" alt="Username=adm Password=Iloveyou" src="https://github.com/user-attachments/assets/ea0f5aa0-5b30-4a19-b7d9-a12d46cdadf0" />
<br>

<br>
  <img width="1093" height="564" alt="Username=Admin Password=12345" src="https://github.com/user-attachments/assets/f66c0502-5d10-4088-a466-666ac2d56e43" />
<br>

<br>
  <img width="1242" height="548" alt="Username=Test Password=12345" src="https://github.com/user-attachments/assets/0279b7c5-50b9-4a51-b721-7f0cb47ba10d" />
<br>

<br>
<img width="1021" height="577" alt="Username=guest Password=12345" src="https://github.com/user-attachments/assets/f5af77bf-6691-4396-8dd7-0d50b927fbfb" />
<br>

<br>
<img width="1029" height="536" alt="Username=info Password=12345" src="https://github.com/user-attachments/assets/3ff21ce1-a809-44a1-a250-9439fafffe24" />
<br>

<br><hr><br>

## There was a successful Brute Force login. The correct Username was Admin and the correct Password was Password.

<h3>This logon happened at 2:15pm. </h3>
<br>
<img width="1072" height="548" alt="Username=admin Password=password" src="https://github.com/user-attachments/assets/007bda10-84ef-4a43-871b-5fde4672b9ef" />
<br>

<h3>The Proxy Log shows that a successful logon occured at 2:15pm</h3>
<br>
<img width="1236" height="491" alt="User Login Successful" src="https://github.com/user-attachments/assets/29d139e3-b00d-46aa-a29b-b7935c7d3817" />
<br>


# Conclusion
## This was a successful Brute Force attempt. The extent of damage done after the bad actor gained access is hard to determine but it is clear that this Endpoint needed to be isolated from the network. 


