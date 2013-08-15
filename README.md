#YHCPickerView

![image](https://dl.dropboxusercontent.com/u/1655028/pickenerimage.png)


##YHCPickerView

If you want to customize elements/list in UIPickerView then YHCPickerView is for you. 

##Features
Compared to the original project, I made ​​changes useful for another project of mine:
* ToolBar color is the same respect UIPickerView
* animation is the same like UIPickerView
* background alpha & color like UIPickerView
* remove search function (but is very simple to reimplement)

##How To

* Drag the `YHCPickerView` to your project


``` objective-c

- (IBAction)btnShowPickerClick:(id)sender {
    

    YHCPickerView *objYHCPickerView = [[YHCPickerView alloc] initWithFrame:CGRectMake(0, 0, 320, 480) withNSArray:countriesArray];
    
    objYHCPickerView.delegate = self;
    [self.view addSubview:objYHCPickerView];
    [objYHCPickerView showPicker];
}

-(void)selectedRow:(int)row withString:(NSString *)text{
    
    NSLog(@"%d",row);
    lblIndex.text = [NSString stringWithFormat:@"%d",row];
    lblText.text = text;
    
}

```

##License

YHCPickerView is available under the MIT License.

Copyright (c) 2012 Yashesh Chauhan

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.

## Credits

Original YHCPickerView was created by [Yashesh Chauhan](https://github.com/yashesh87) 
