	

    import java.util.Arrays;
    import java.util.Scanner;
     
     
    public class TaweeLab {
     
            public static void main(String[] args) {
                    int first=100000,sec=100000,thr=100000,forth=100000;
                    Scanner scan = new Scanner(System.in);
                    System.out.print("Enter first dimension : ");
                    int firstDimension = scan.nextInt();
                    System.out.print("Enter second dimension : ");
                    int secondDimension = scan.nextInt();
                    System.out.print("Enter third dimension : ");
                    int thirdDimension = scan.nextInt();
                    System.out.print("Enter forth dimension : ");
                    int forthDimension = scan.nextInt();
                    int[][][][] ArrayT = new int[firstDimension][secondDimension][thirdDimension][forthDimension];
     
                    while(true){
                           
                            while(first>=firstDimension){
                            System.out.print("Enter first location : ");
                            first = scan.nextInt();
                            if(first<firstDimension){
                                    break;
                            }
                            }
                            if(first<0){
                                    break ;
                            }
                           
                            while(sec>=secondDimension){
                            System.out.print("Enter second location : ");
                            sec = scan.nextInt();
                            if(sec<secondDimension&&sec>=0){
                                    break;
                            }
                            }
                           
                            while(thr>=thirdDimension){
                            System.out.print("Enter third location : ");
                            thr = scan.nextInt();
                            if(thr<thirdDimension&&thr>=0){
                                    break;
                            }
                            }
                           
                            while(forth>=forthDimension){
                            System.out.print("Enter forth location : ");
                            forth = scan.nextInt();
                            if(forth<forthDimension&&forth>=0){
                                    break;
                            }
                            }
                            System.out.print("Enter number : ");
                            int number = scan.nextInt();
                            ArrayT[first][sec][thr][forth] = number;
                    }
                           
                   
                    for(int i =0;i<ArrayT.length;i++){
                            System.out.print("{{{");
                            for(int j =0;j<ArrayT[0].length;j++){
                                    System.out.print("---");
                                    for(int k=0;k<ArrayT[0][0].length;k++){
                                            System.out.print(Arrays.toString(ArrayT[i][j][k]));
                                    }
                                    System.out.print("---");
                                   
                            }
                            System.out.print("}}}");
                            System.out.println();
                    }
                    //System.out.println(Arrays.toString(ArrayT[0][0]));
                    //System.out.println(Arrays.toString(ArrayT[1]));
                    //System.out.println(Arrays.toString(ArrayT[2]));
                   
            }
     
    }

