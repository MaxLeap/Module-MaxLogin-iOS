# Module-MaxLogin-iOS

MaxLoginUI.embededframework集成了MaxLeap登陆界面，直接初始化ViewController就可以进行MaxLeap用户注册、登录，或者第三方登录。

使用方法：

1、MaxLeap用户登录


	MCLoginViewController *loginViewController = [[MCLoginViewController alloc]init];
    UINavigationController *loginNavigationController = [[UINavigationController alloc]initWithRootViewController:loginViewController];
    [self presentViewController:loginNavigationController animated:YES completion:nil];
    
2、MaxLeap用户注册

    MCSignViewController *signViewController = [[MCSignViewController alloc]init];
    signViewController.signType = MaxChatSignUp;
    UINavigationController *signNavigationController = [[UINavigationController alloc]initWithRootViewController:signViewController];
    [self presentViewController:signNavigationController animated:YES completion:nil];
    
3、第三方登录


    MCSignViewController *signViewController = [[MCSignViewController alloc]init];
    signViewController.signType = MaxChatSignIn;
    UINavigationController *signNavigationController = [[UINavigationController alloc]initWithRootViewController:signViewController];
    [self presentViewController:signNavigationController animated:YES completion:nil];