# aws-elasticBeanStack
elasticBeanStack deployment 

https://medium.com/@xoor/deploying-a-node-js-app-to-aws-elastic-beanstalk-681fa88bac53

set PORT = 8081 default accepted by nginx reverse proxy server to proxy to port 80 // default by http

set the health check route for load balancer
// default to /
app.get('/', (req, res)=>{res.status(200).send()})

with webSockets
https://levelup.gitconnected.com/beginners-guide-to-aws-beanstalk-using-node-js-d061bb4b8755

with .ebextensions for env variable files -- create 3 for dev prod test
https://medium.freecodecamp.org/how-to-deploy-a-node-js-app-to-the-aws-elastic-beanstalk-f150899ed977
