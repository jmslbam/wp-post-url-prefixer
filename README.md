# WordPress post url prefixer
Prefix only your post URL and not your tag and category permalinks & have a automatic blog posts archive


## Change singular post prefix
```
add_filter('wp_pup_singular_prefix', function(){
	return 'news';
});
```

## Change the post archive slug

### Change the post archive slug
``` 
add_filter('wp_pup_archive_slug', function(){
	return 'news';# 
});
```

### Disable the automaticly enable post archive
``` 
add_filter('wp_pup_archive_slug', function(){
	return false;
});
```