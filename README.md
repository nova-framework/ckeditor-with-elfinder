# ckeditor-with-elfinder
standalone ckeditor with integrated elfinder out the box

## Usage:

add the js file:

ckeditor/ckeditor.js

````
Assets::js(array(
    site_url('ckeditor/ckeditor.js')
));
````

set path to elfinder:

````
CKEDITOR.editorConfig = function( config ) {
  config.filebrowserBrowseUrl = '<?=site_url();?>admin/editor';
  config.baseHref = '<?=site_url();?>';
};
````
