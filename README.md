# docker-settings-for-widows10
While running the Docker in Winodws 10
Error:
```
An error occured
Failed to create of configure Hyper-V VM: Sequence contain no elements
```

1. Open Windows Security -> App Browser control -> Click on "Exploit protection Settings" -> Open "Proram Settings" Tab
2. Check for "C:\Windows\Systmen32\vmcompute.exe"
3. Click on Edit
4. Uncheck All check boxes
5. Open Powershell in Admin mode
6. Run "net start vmcompute". It should say "The Hyper-V Host Compute Service service was started successfully."
7. Run the docker app
