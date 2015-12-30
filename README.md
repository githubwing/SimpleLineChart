# CirclePercentView
An Android simple LineChart 
<<<<<<< HEAD
=======
博客讲解地址http://blog.csdn.net/wingichoy/article/details/50434634
###Perview
![image](https://github.com/githubwing/CirclePercentView/raw/master/perview.jpg)
###How To Use
Add a SimpleLineChart into your XML.

```
<com.wingsofts.simplelinechart.SimpleLineChart
    android:id="@+id/simpleLineChart"
    android:layout_width="400dp"
    android:layout_height="200dp" />
```
You must set XAxis item and YAxis item and dataSource like:
```
 mSimpleLineChart = (SimpleLineChart) findViewById(R.id.simpleLineChart);
        String[] xItem = {"1","2","3","4","5","6","7"};
        String[] yItem = {"10k","20k","30k","40k","50k"};
        if(mSimpleLineChart == null)
            Log.e("wing","null!!!!");
        mSimpleLineChart.setXItem(xItem);
        mSimpleLineChart.setYItem(yItem);
        HashMap<Integer,Integer> pointMap = new HashMap();
        for(int i = 0;i<xItem.length;i++){
            pointMap.put(i, (int) (Math.random()*5));
        }
        mSimpleLineChart.setData(pointMap);
```
