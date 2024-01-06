```
class Solution {
    public List<List<Integer>> threeSum(int[] nums) {
        List<List<Integer>> list = new ArrayList<>();
        Map<Integer, Integer> map = new HashMap<>();
        Set<List<Integer>> set = new HashSet<>();
        int n = nums.length;
        for(int i = 0; i < n - 1; i++) {
            {
                int target = 0 - (nums[i]);
                for(int j = i + 1; j < n; j++) {
                    if(map.containsKey(target - nums[j])) {
                        List<Integer> list1 = new ArrayList<>(Arrays. asList(nums[i], target - nums[j], nums[j]));
                        List<Integer> list2 = new ArrayList<>();
                        Collections.sort(list1);
                        list2.add(list1.get(0));
                        list2.add(list1.get(1));
                        list2.add(list1.get(2));
                        if(!set.contains(list2))
                            list.add(list2);
                        set.add(list1);
                    } else {
                        map.put(nums[j], j);
                    }
                }
                map.clear();
            }
        }
        return list;
    }
}
```
