UITextField-Shake
=================

UITextField摇晃，可用于提示


// 调用方法，_textField将shake5次

    [_textField shake:10 withDelta:5 andSpeed:0.04];



// 统一改变textfield边框颜色或者宽度的方法。

// 利用NSArray的enumerateObjectUsingBlock方法。

NSArray *fields = @[_textShake, _textSpeed, _textDelta, _textField];
    [fields enumerateObjectsUsingBlock:^(UITextField *obj, NSUInteger idx, BOOL *stop){
        [obj.layer setBorderWidth:2];
        [obj.layer setBorderColor:[UIColor colorWithRed:49.0/255.0 green:186.0/255.0 blue:81.0/255.0 alpha:1].CGColor];
    }];
}
