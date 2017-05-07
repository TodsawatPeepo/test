# test
แบบฝึก
import java.io.BufferedReader;
import java.io.FileReader;
import java.io.IOException;

public class HR {
	public static void main(String[] args) {
		
		BufferedReader in = null;
		try{
			in = new BufferedReader(new FileReader("E:/Users/Lampo 'San/workspace/Dev_Test_2016/1.working_time.log"));
			String read = null;
			String n = "/+s";
			while((read = in.readLine()) != null){
				String[] splited = read.split("\\|");
				String[] parts = null;
				
				for(String part : splited){
					System.out.println("______________________");
					System.out.println("Spliter 0 ="+splited[0]);
					System.out.println("Spliter 1 ="+splited[1]);
					System.out.println("Spliter 2 ="+splited[2]);
					System.out.println("Spliter 3 ="+splited[3]);
					System.out.println("Spliter 4 ="+splited[4]);
					System.out.println("______________________");
					break;
				}
				if(splited[0].equals("น.ส.เรวดี ประสพศิลป")){
					System.out.println("______________________");
					System.out.println("Spliter 0 ="+splited[0]);
					System.out.println("Spliter 1 ="+splited[1]);
					System.out.println("Spliter 2 ="+splited[2]);
					System.out.println("Spliter 3 ="+splited[3]);
					System.out.println("Spliter 4 ="+splited[4]);
					System.out.println("______________________");
				}
				
			}
			
		}catch (IOException e){
			System.out.println("ERROR PLEAS TRY AGAIN!!!" + e);
			e.printStackTrace();
		}finally{
			try{
				in.close();
			}catch(Exception e){
				
			}
		}
	}
}
	
