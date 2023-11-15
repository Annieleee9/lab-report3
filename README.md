# lab-report3
```
@Test
  public void averageWithoutLowest() {
    double [] input1 = {2.5,2.5,1.5,3.5};
    assertEquals(5, ArrayExamples.averageWithoutLowest(input1),0);
  }
```
```
  @Test
  public void averageWithoutLowest2() {
    double [] input1 = {0, 0,0, 0};
    assertEquals(0, ArrayExamples.averageWithoutLowest(input1),0);
  }
```
```
static double averageWithoutLowest(double[] arr) {
    double total=0;
    if(arr.length < 2) { 
      return 0.0; }
    double lowest = arr[0];
    for(double num: arr) {
      if(num < lowest) { 
        lowest = num; }
    }
    double sum = 0;
    for(double num: arr) {
      if(num != lowest) { 
        sum += num; }
    }
    return sum/(arr.length-1);
  }
```
```
  static double averageWithoutLowest(double[] arr) {
    double total=0;
    if(arr.length < 2) { 
      return 0.0; }
    double lowest = arr[0];
    for(double num: arr) {
      if(num < lowest) { 
        lowest = num; }
    }
    double sum = 0;
    for(double num: arr) {
      if(num != lowest) { 
        sum += num; }
    }
    
      total = sum / (arr.length-1);
      double roundOff = Math.round(total*100.0)/100.0;
    return (roundOff);
  }
```
