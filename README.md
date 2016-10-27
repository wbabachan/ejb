# ejb
This is a small and very simple example for the people who wants to learn Java EE EJB technology. It covers EJB stateless session beans, JPA Entity beans, JMS Point-to-Point Message transport and CDI Interceptors.

The Code is very small and lightweight and aims the developer that wants to understand how EJBs are working. 

In order to test the code, you have to import it in Intellij or Eclipse IDE and add CDI, JMS, JPA and JavaEE capability, e.g. in Intellij by selecting them in "Add Framework" on context Menu of imported Project. Furthermore you have to use and configure an Application Server. You have to create JDBC Pool and JNDI Resource, JMS Messaging factory and JMS Resource. 

JTA-Data-Source on Server must be named as "jdbc/ejb"

JMS-Data-Source must have the following properties: \
destination **ejbQueue** \
destinationType **javax.jms.Queue**

JMS Connection factory must be named as **jms/__defaultConnectionFactory** \
JMS Queue **jms/ejbqueue**

After configuring the application server, you have to start it and run the servlet in ejb-client project.

Enjoy it !
