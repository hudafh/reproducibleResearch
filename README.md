# reproducibleResearch

study <- function() {
        
        
        activityData <- read.csv("./activity.csv")
        
        daily <- summarise(group_by(activityData, date,interval,steps))
        colnames(daily) <- c("date", "interval","steps")
        
        daily
        #BEGINING
        #nrNAs <- length(is.na(daily))
        
        #noNAs <- !is.na(daily[,"steps"])
        
        #daily <- daily[noNAs,]
        
        #total_steps_by_day <- summarise( group_by(daily,date), sum(steps))
        #colnames(total_steps_by_day) <- c("date", "steps")
        #total_steps_by_day
        
        #days <- as.POSIXct(total_steps_by_day$date, format = '%Y-%m-%d')
        
        #hist(total_steps_by_day$steps, col = "red")  #plot histogram
        
        #avg_steps_day <- mean(total_steps_by_day$steps)
        
        #median_steps_day <- median(total_steps_by_day$steps)
        
        #print(avg_steps_day)
        #print(median_steps_day)
        
        #total_steps_by_day
        
        #interval_avg <- summarise(group_by(daily,interval), mean(steps))
        #colnames(interval_avg) <- c("interval","steps")
        #plot(interval_avg$interval,as.numeric(interval_avg$steps), type = "l")
        
        #interval_avg
        #END
        #interval 835 has the highest average of steps
        
        
        
        #days
        #interval average steps
        #interval_avg_steps <- summarise(group_by(steps_by_day,interval), mean(steps))
        #colnames(interval_avg_steps) <- c("interval","steps")
        
        #interval_avg_steps
        
        #max(interval_avg_steps$steps)
        #days <- as.POSIXct(steps_by_day$date, format = '%Y/%m/%d')
        
       # days
        #png("./g1.png")
        
        #plot(days,total_steps_by_day$steps, type = "l")
        #dev.off()
        
        #steps_by_day
        
      #  stepsMean <- mean(steps_by_day$steps)
        
      #  stepsMedian <- median(steps_by_day$steps)
        
        
        
}
