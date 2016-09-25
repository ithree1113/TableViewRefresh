# TableViewRefresh

## Screenshot
![MacDown Screenshot] (https://raw.githubusercontent.com/ithree1113/TableViewRefresh/master/ScreenShot/exam.png)

## Usage
Add code that you want to do during refreshing in the function below.

```objc
-(void)tableViewRefresh {    
    NSLog(@"Refresh starts");
    
    [self.refresh endRefreshing];
    NSLog(@"Refresh ends");
}

```

## License
TableViewRefresh_DEMO is available under the MIT license. See the [LICENSE](https://raw.githubusercontent.com/ithree1113/TableViewRefresh_DEMO/master/LICENSE) file for more info.