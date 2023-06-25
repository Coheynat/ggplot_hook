#loading the relevent libraries.
library(ggplot2)
library(palmerpenguins)

#add a title to the graph.
ggplot(data=penguins)+
  geom_point(mapping=aes(x=flipper_length_mm,y=body_mass_g,color=species))+
  labs(title="Palmer Penguins: Body Mass vs. Flipper Length")

#add a subtitle.
ggplot(data=penguins)+
  geom_point(mapping=aes(x=flipper_length_mm,y=body_mass_g,color=species))+
  labs(title="Palmer Penguins: Body Mass vs. Flipper Length", subtitle="Sample of Three Penguin Species")

#Add a caption. Caption let us show the source of the data. 
ggplot(data=penguins)+
  geom_point(mapping=aes(x=flipper_length_mm,y=body_mass_g,color=species))+
  labs(title="Palmer Penguins: Body Mass vs. Flipper Length", subtitle="Sample of Three Penguin Species", caption="Data collected by Dr. Kristen Gorman")

#Titles, subtitles and captions are labels that we pust outside of the grid of our plot to indicate important information.
#adding text inside the data grid to call out important data code using the "annotate" function.

#add annotation. 
ggplot(data=penguins)+
  geom_point(mapping=aes(x=flipper_length_mm,y=body_mass_g,color=species))+
  labs(title="Palmer Penguins: Body Mass vs. Flipper Length", subtitle="Sample of Three Penguin Species", caption="Data collected by Dr. Kristen Gorman")+
annotate("text",x=220,y=3500,label="The Gentoos are the largest")

#add color to an annotation.
ggplot(data=penguins)+
  geom_point(mapping=aes(x=flipper_length_mm,y=body_mass_g,color=species))+
  labs(title="Palmer Penguins: Body Mass vs. Flipper Length", subtitle="Sample of Three Penguin Species", caption="Data collected by Dr. Kristen Gorman")+
  annotate("text",x=220,y=3500,label="The Gentoos are the largest",color="purple")

#change font style and size.
ggplot(data=penguins)+
  geom_point(mapping=aes(x=flipper_length_mm,y=body_mass_g,color=species))+
  labs(title="Palmer Penguins: Body Mass vs. Flipper Length", subtitle="Sample of Three Penguin Species", caption="Data collected by Dr. Kristen Gorman")+
  annotate("text",x=220,y=3500,label="The Gentoos are the largest",color="pink",fontface="bold", size=3.0)

#change the angle of the text. Tilting it in 25 dgrees.
ggplot(data=penguins)+
  geom_point(mapping=aes(x=flipper_length_mm,y=body_mass_g,color=species))+
  labs(title="Palmer Penguins: Body Mass vs. Flipper Length", subtitle="Sample of Three Penguin Species", caption="Data collected by Dr. Kristen Gorman")+
  annotate("text",x=220,y=3500,label="The Gentoos are the largest",color="green",fontface="bold", size=3.0,angle=25)

#store the plot as a variable and than adding an anotation, to keep code tidy and easier to understand. 
#calling the plot "p":
p <- ggplot(data=penguins)+
  geom_point(mapping=aes(x=flipper_length_mm,y=body_mass_g,color=species))+
  labs(title="Palmer Penguins: Body Mass vs. Flipper Length", subtitle="Sample of Three Penguin Species", caption="Data collected by Dr. Kristen Gorman")

#add annotation to a variable:
p+annotate("text",x=220,y=3500,label="The Gentoos are the largest",color="gold",fontface="italic", size=3.0,angle=25)

#save our work via the ggsave()
ggsave("PalmerPenguins_viz_R.png")
