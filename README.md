# wordcloud
#主要记录文字云的绘制过程
data22<- read.table('clipboard',T)
library(wordcloud)
wordcloud(words=data22$word,freq=data22$freq,col=rainbow(length(data22$freq)))
#wordcloud2
library(wordcloud2)
wordcloud2(data22)
