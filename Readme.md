# docker-crontab-sample
- How to run
```sh
# build and run docker
> sudo docker build --rm -t docker-crontab-sample .
> sudo docker run -it docker-crontab-sample

# in docker, wait one minutes
> crontab -l   
* * * * * echo "Hell0 w0r1d for yOu" >> /var/log/cron.log
cat /var/log/cron.log 
> Hell0 w0r1d for yOu 

```


- ref: English https://stackoverflow.com/questions/37458287/how-to-run-a-cron-job-inside-a-docker-container
- ref: Chinese https://www.jianshu.com/p/351a2b2b416b
