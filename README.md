# TableViewRefresh
This is a simple demo for TableView refresh when user pull down the table.

## Screenshot
![MacDown Screenshot] (https://raw.githubusercontent.com/ithree1113/TableViewRefresh/master/ScreenShot/exam.png)

## Setup
```objc
@property (nonatomic) UIRefreshControl *refresh;
```

```objc
self.refresh = [[UIRefreshControl alloc]init];
[self.refresh addTarget:self action:@selector(tableViewRefresh) forControlEvents:UIControlEventValueChanged];
[self.tableView addSubview:self.refresh];
```
But this object is ONLY available with Table View Controller.


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