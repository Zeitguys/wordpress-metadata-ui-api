# Code Architecture


    $form = WP_Form( {
        'id' => 'my-id', // Optional, could be auto-generated. Not really needed, other than for CSS purposes
        'post_types' => array( 'post', 'page', 'my-cpt-slug' ), // Optional. Auto-registers metabox for these post types
        'metabox_callback' => array( $this, 'my_metabox_cb' ), // Optional. Used to override default metabox behaviour
        'save_post_callback' => array( $this, 'my_save_post_cb' ), // Optional. Used to override default meta save
    } );

