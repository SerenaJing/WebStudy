# JavaScript排序算法
# 1. 冒泡排序
# 最快（Best Cases）：当输入的数据已经是正序时
# 最慢（Worst Cases）：当输入的数据是反序时
function bubbleSort(arr) {
    var len = arr.length;
    for (var i = 0; i < len; i++) {
        for (var j = 0; j < len - 1 - i; j++) {
            if (arr[j] > arr[j+1]) {        //相邻元素两两对比
                var temp = arr[j+1];        //元素交换
                arr[j+1] = arr[j];
                arr[j] = temp;
            }
        }
    }
    return arr;
}
