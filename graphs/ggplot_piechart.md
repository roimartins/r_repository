### create a ggplot pie char in R . Include labelling. 

```r
ggplot( ff  , aes(y= catch_ratio_total_site, x= "", fill= factor(nn)    )) +   scale_fill_brewer(palette = "Set3")  +
  geom_bar( width = 0.5, stat ="identity") +
  cp + 
  blank_theme +
  theme(axis.text.x=element_blank()) +
  geom_text( aes(label = percent( catch_ratio_total_site )  ) ,size = 3, position = position_stack(vjust = 0.5)) +
  facet_grid(~site_name,  scales = "free" ) 


```
