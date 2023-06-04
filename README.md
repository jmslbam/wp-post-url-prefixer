# WordPress post url prefixer
Prefix only your post URL and not your tag and category permalinks & have a automatic blog posts archive


## Change singular post prefix
Defaults to `/blog/` like https://jaimemartinez.nl/blog/using-twig-in-wordpress-with-clarkson/

```
add_filter('wp_pup_singular_prefix', function(){
	return 'news';
});
```

## Change the post archive slug

Defaults to https://jaimemartinez.nl/blog/ if you have not selected a page for the "Reading settings > Posts page" setting.
If you want to change it, the use this filter:

### Change the post archive slug
``` 
add_filter('wp_pup_archive_slug', function(){
	return 'news';
});
```

### Disable the automaticly enable post archive
If you don't want fancy automaticly enabled post archive, then disable it like this:

``` 
add_filter('wp_pup_archive_slug', function(){
	return false;
});
```