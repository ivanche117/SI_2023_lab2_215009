Ивана Стојановска 215009

2. Слика од Control Flow Graph

<img width="393" alt="cfg 215009" src="https://github.com/ivanche117/SI_2023_lab2_215009/assets/127608868/6cb3130c-87d0-4331-bf04-77bc842fc320">



3. Цикломатската комплексност на графот изнесува 11. 
   Оваа вредност ја добив преку пресметување на повеќе начини:
       а) бројот на предикатни јазли + 1 = 10+1 = 1
       б) Број на јазли = 32
          Број на ребра = 41
          41-32+2 = 11
       в) број на региони = 11
       
 4. /
 5. if (user==null || user.getPassword()==null || user.getEmail()==null)
      Бидејќи имаме 1 услов со 3 подуслови (user==null || user.getPassword()==null || user.getEmail()==null) кои што се со или, а 2^3=8, значи треба да имам 8 test cases.
      
      тестовите се:
      user=null, user.getPassword()=null, user.getEmail()=null                                     //(0, 0, 0)
      
      user=user, user.getPassword()="password", user.getEmail()=""email@gmail.com                  //(1, 1, 1)
     
      user=user, user.getPassword()=null, user.getEmail()=""email@gmail.com                        //(1, 0, 1)
    
      user=user, user.getPassword()="password", user.getEmail()=null                               //(1, 1, 0)
    
      user=user, user.getPassword()=null, user.getEmail()=null                                     //(1, 0, 0) 
    
    
    
    
   
      user=null, user.getPassword()="password", user.getEmail()=""email@gmail.com                  //(0, 1, 1)
    
      user=null, user.getPassword()=null, user.getEmail()=""email@gmail.com                        //(0, 0, 1)
    
      user=null, user.getPassword()="password", user.getEmail()=null                               //(0, 1, 0)
     
  Бидејќи во последните 3 услови user=null значи дека објектот не постои, повлекува дека и user.getEmail()=null И user.getPassword()=null ,
  значи дека тие 3 тестови нема да постојат. 
 
        
