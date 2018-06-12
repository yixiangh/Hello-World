# Hello-World
测试存储库
public static void main(String[] args) {
		List<String> list = new ArrayList<String>();
		for (int i = 0; i < 1090; i++) {
			list.add(i+"");
		}
		System.out.println("大小："+list.size());
		int times = (int)Math.ceil( list.size()/200.0 );
		System.out.println("times:"+times);
	    for(int i=0; i<times; i++ ){
	        System.out.println("a："+ Math.min((i+1)*200, list.size()-1));
	        System.out.println(list.subList(i*200, Math.min((i+1)*200, list.size()-1)));
	    }
	}
