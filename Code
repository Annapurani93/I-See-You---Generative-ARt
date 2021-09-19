library(aRtsy)
library(tidyverse)
library(magick)
set.seed(2)

#Creating the eyes
colors <- list(c("#036d87", "#050914"), "#070B18", "#fafafa","#070B18")

canvas_planet(colors, radius = c(500, 150, 25, 10),
              center.x = c(750, 750, 750, 750),
              center.y = c(750, 750, 750, 750),
              fade=0.01)->a

ggsave("a.png", a, width = 18, height = 18)


colors <- list(c("#02a7cc","#0D98BA","#fafafa"), "#070B18", "#fafafa","#070B18")
               
canvas_planet(colors, radius = c(500, 150, 25, 10),
                             center.x = c(750, 750, 750, 750),
                             center.y = c(750, 750, 750, 750),
                             fade=0.01)->a1

ggsave("a1.png", a1, width = 18, height = 18)

colors <- list(c("#fa2100","#fafafa"), "#070B18", "#fafafa","#070B18")

canvas_planet(colors, radius = c(500, 150, 25, 10),
              center.x = c(750, 750, 750, 750),
              center.y = c(750, 750, 750, 750),
              fade=0.01)->a2

ggsave("a2.png", a2, width = 18, height = 18)


colors <- list(c("#94c24f", "#8c7803"), "#070B18", "#fafafa","#070B18")

canvas_planet(colors, radius = c(500, 150, 25, 10),
              center.x = c(750, 750, 750, 750),
              center.y = c(750, 750, 750, 750),
              fade=0.01)->a3

ggsave("a3.png", a3, width = 18, height = 18)

#Reading and resizing the image
a<- image_read('C:/Users/Annapurani/Desktop/a.png')
a1 <- image_read("C:/Users/Annapurani/Desktop/a1.png")
a2<- image_read('C:/Users/Annapurani/Desktop/a2.png')
a3<- image_read("C:/Users/Annapurani/Desktop/a3.png")
image_scale(a, "300x300")->a
image_scale(a1, "300x300")->a1
image_scale(a2, "300x300")->a2
image_scale(a3, "300x300")->a3

#To annotate
a%>%image_annotate("@annapurani93", size = 12, color = "white", location = "+200+280")->a
a1%>%image_annotate("@annapurani93", size = 12, color = "white", location = "+200+280")->a1
a2%>%image_annotate("@annapurani93", size = 12, color = "white", location = "+200+280")->a2
a3%>%image_annotate("@annapurani93", size = 12, color = "white", location = "+200+280")->a3

#To save the final image
image_write(a, path = "final11.png", format = "png") 
image_write(a1, path = "final12.png", format = "png") 
image_write(a2, path = "final13.png", format = "png") 
image_write(a3, path = "final14.png", format = "png") 
