### 概述
自建OAuth2认证服务

内置了两个用户   
SecurityConfiguration：
```
...
.withUser("user").password(passwordEncoder().encode("user")).roles("USER")
.and().withUser("admin").password(passwordEncoder().encode("admin")).roles("ADMIN");
...
```

