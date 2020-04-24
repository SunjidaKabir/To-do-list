package to.pkgdo.list;
import java.util.Date;
import java.util.Scanner;
public class Task extends Date
{
	private int id; 
	private String taskName;
	private boolean isDone; 
	private Date taskCreated, taskCompleted, deadline; 
	private static int autoIncrementingId = 1;

	public Task(String taskName, Date deadline)
        {
		this.taskName = taskName;
		id = autoIncrementingId++;
		this.deadline = deadline;
		isDone = false;
		taskCreated = new Date();
	}
    
    public void setId(int id)
    {
        this.id = id;
    }
    
    public int getId() 
    {
        return id;
    }
   
    
    public void setTaskName(String taskName)
    {   
        if(taskName.length()<10)
        {
             this.taskName =taskName;
        }
       
    }
    
    public String getTaskName() 
    {
        return taskName;
    }
    
    

    public void setIsDone(boolean isDone)
    {
        this.isDone = isDone;
    }
    
    
    public boolean isIsDone()
    {
        return isDone;
    }
    
    


    public void setTaskCreated(Date taskCreated) 
    {
        this.taskCreated = taskCreated;
    }
    
    public Date getTaskCreated()
    {
        return taskCreated;
    }
    
    


    public void setTaskCompleted(Date taskCompleted) 
    {
        this.taskCompleted = taskCompleted;
    }
    
    
    public Date getTaskCompleted()
    {
        return taskCompleted;
    }
    
    



    public void setDeadline(Date deadline)
    {
        this.deadline = deadline;
    }
    
    public Date getDeadline() 
    {
        return deadline;
    }
    
    
    
    public static void main(String[] args)
    {
        
    }
    
}
