
public class RandomNumber 
{
  private int lowBound;
  private int hiBound;
  
  public RandomNumber()
        
  {
    lowBound = 1;
    hiBound = 10;
  }
                      
  public RandomNumber (int low, int high) 
  {
    lowBound = low;
    hiBound = high;
  }
                                                    
  public int  GetANumber_Between_1_and_10()
  {
    int randNum;
    randNum = (0+ (int)(Math.random() * 10));
    return randNum;
  }
                                                                                            
  public int GetANumber()
  {
    int compNum = lowBound + (int) (Math.random() * hiBound);
    return compNum;
  }
                                                                                                            
}
                                                                                                            
//=========================================
public class DisplayNumber 
{
  public static void main( String[] args)
    {
      RandomNumber randNum   = new RandomNumber();
      System.out.printf("The random number is:  %d", randNum.GetANumber());
    }
}
                                                                                                                                        
