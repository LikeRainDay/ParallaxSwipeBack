  Android ParallaxSwipeBack
=======================

带视觉差的侧滑返回，类似于新版微信和lofter的侧滑返回效果。核心代码小于50行.  
![image](https://github.com/bushijie/ParallaxSwipeBack/blob/master/show.gif) 

Usage
-----
 `public class MainActivity extends ParallaxSwipeBackActivity {

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_main);
        findViewById(R.id.next).setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View v) {
                Intent intent = new Intent(MainActivity.this,NextActivity.class);
                intent.putExtra("index",0);
                startParallaxSwipeBackActivty(MainActivity.this, intent);
            }
        });

    }`   



