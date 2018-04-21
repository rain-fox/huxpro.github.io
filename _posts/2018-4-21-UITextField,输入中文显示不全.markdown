---
layout:     post
title:      "UITextField 输入中文时左侧显示bug"
subtitle:   " \"UITextField 输入中文时左侧边框遮挡文字\""
date:       2018-04-21 15:00:00
author:     "Rain-fox"
header-img: "img/HelloWorld.png"
catalog: true
tags:
    iOS
--- 

> “UITextField 输入中文时左侧显示bug”

## 正文

> “UITextField 输入中文时左侧显示bug”

UITextField 在使用autoLayout,并且没有限定宽度的时候，输入中文的时候会出现左侧文字显示不全。

UILabel * leftView = [[UILabel alloc] initWithFrame:CGRectMake(0,0,8,25)];
leftView.backgroundColor = [UIColor clearColor];
_textField.leftView = leftView;
_textField.leftViewMode = UITextFieldViewModeAlways;

只需要在使用UITextView的leftView，并且设置leftViewMode = UITextFieldViewModeAlways即可



