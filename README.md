finction the_function_name(){
	load_theme_textdomain( 'textdomain_name', get_template_directory() . '/languages' );
	
	add_theme_support( 'title-tag' );
	
	add_theme_support( 'automatic-feed-links' );
	
	add_theme_support( 'custom-logo', array(
			'height'      => 240,
			'width'       => 240,
			'flex-height' => true,
		) );
	
	add_theme_support( 'post-thumbnails' );
	
	set_post_thumbnail_size( 1200, 9999 );
	
	add_theme_support( 'html5', array(
		'search-form',
		'comment-form',
		'comment-list',
		'gallery',
		'caption',
	) );
	
	add_theme_support( 'post-formats', array(
	'aside','image',	'video','quote','link','gallery',	'status','audio','chat',
	) );
	
	add_theme_support( 'customize-selective-refresh-widgets' );
}
add_action('after_setup_theme', 'the_function_name');
