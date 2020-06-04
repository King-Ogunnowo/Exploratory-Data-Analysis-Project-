To fill in missing values in SQL
```
select location_region, location_state from ad_dataset;
update ad_dataset
set location_region = '' where location_state = '';
```

To select the right part of a string after a specific character 
```
select site_name, site_link from ad_dataset;
select substring_index (site_link, '/',3) from ad_dataset limit 201859;
```

To count a variable in excel 
```
countif(ad_dataset!a2:a201858, ' ')
```

To count two variables in excel 
```
countifs(ad_dataset!a2:a201858, ' ', ad_dataset!b2:b201858, ' ')
```

To retrieve the left part of a string in excel 
```
left(O2,10)
```

To retrieve a the mid value of in a string in excel 
```
mid(o2,12,2)
```

To calculate the average in excel
```
=average(a2:a201858)
```
