# jenkins-rolebases-user

Follow the steps given in below url

[Adding User](https://www.guru99.com/create-users-manage-permissions.html)

Once you add the user and configured Global security for role based strategy, the jenkins wont work,

# So do the below change in config.xml under /var/lib/jenkins 

```
Step1:  
      <useSecurity>true</useSecurity>  change it to false
      <useSecurity>false</useSecurity>
      
Step2:
      Comment out the <authorizationStrategy> part 

Step3: 
      Restart the jenkins service
      
```

