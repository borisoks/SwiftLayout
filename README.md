# SwiftLayout

```
class ViewController: UIViewController {

    override func viewDidLoad() {
        super.viewDidLoad()
        // Do any additional setup after loading the view, typically from a nib.
        
        //Setup views
        
        let v1 = UIView()
        v1.backgroundColor = UIColor.purple
        self.view.addSubview(v1)
        
        let v2 = UIView()
        v2.backgroundColor = UIColor.blue
        self.view.addSubview(v2)
        
        let v3 = UIView()
        v3.backgroundColor = UIColor.orange
        self.view.addSubview(v3)
        
        let v4 = UIView()
        v4.backgroundColor = UIColor.orange
        self.view.addSubview(v4)

        
        // Layout using SwiftLayout
        
        v1.layout.top(0, anchor: self.topLayoutGuide.bottomAnchor).right(5).height(50).left(5)
        v2.layout.top(5, anchor: v1.anchors.bottom).right(5).height(50).left(5)
        
    }

}
```
