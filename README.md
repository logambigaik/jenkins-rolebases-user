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


>>    or Follow below method:
Go to Manage Jenkins > Configure Global Security and select the Enable Security checkbox.

![image](https://user-images.githubusercontent.com/54719289/119489658-cf225100-bd53-11eb-96e7-3354bd28e291.png)

