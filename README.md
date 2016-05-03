flickr document

https://www.flickr.com/services/api/auth.howto.web.html\

https://www.flickr.com/services/api/auth.oauth.html

![alt tag](https://raw.githubusercontent.com/0way/phpflickr/master/hinh_mieuta.png)

List Class and funtion important in  phpFlickr.php

Class phpFlickr {
  function phpFlickr ($api_key, $secret = NULL, $die_on_error = false) {
  function enableCache ($type, $connection, $cache_expire = 600, $table = 'flickr_cache') {
  function getCached ($request)
  function cache ($request, $response)
  function setCustomPost ( $function ) {
  function setCustomPost ( $function ) {
  
  function post ($data, $type = null) {
  
  function request ($command, $args = array(), $nocache = false)
  function clean_text_nodes ($arr) {
  function setToken ($token) {
  function setProxy ($server, $port) {
  function getErrorCode () {
  function getErrorMsg () {
  function buildPhotoURL ($photo, $size = "Medium") {
  function sync_upload ($photo, $title = null, $description = null, $tags = null, $is_public = null, $is_friend = null, $is_family = null) {
  
  function async_upload ($photo, $title = null, $description = null, $tags = null, $is_public = null, $is_friend = null, $is_family = null) {
  
  function replace ($photo, $photo_id, $async = null) {
  
  function auth ($perms = "read", $remember_uri = true) {
  function auth_url($frob, $perms = 'read') {
  function call ($method, $arguments) {
  
  
  function activity_userComments ($per_page = NULL, $page = NULL) {
  function activity_userPhotos ($timeframe = NULL, $per_page = NULL, $page = NULL) {
  function auth_checkToken () {
  function auth_getFrob () {
  function auth_getFullToken ($mini_token) {
  function auth_getToken ($frob) {
  function blogs_getList ($service = NULL) {
  function blogs_getServices () {
  function blogs_postPhoto ($blog_id = NULL, $photo_id, $title, $description, $blog_password = NULL, $service = NULL) {
  function collections_getInfo ($collection_id) {
  function collections_getTree ($collection_id = NULL, $user_id = NULL) {
  function commons_getInstitutions () {
  function contacts_getList ($filter = NULL, $page = NULL, $per_page = NULL) {
  function contacts_getPublicList ($user_id, $page = NULL, $per_page = NULL) {
  function contacts_getListRecentlyUploaded ($date_lastupload = NULL, $filter = NULL) {
  function favorites_add ($photo_id) {
  function favorites_getList ($user_id = NULL, $jump_to = NULL, $min_fave_date = NULL, $max_fave_date = NULL, $extras = NULL, $per_page = NULL, $page = NULL) {
  function favorites_getPublicList ($user_id, $jump_to = NULL, $min_fave_date = NULL, $max_fave_date = NULL, $extras = NULL, $per_page = NULL, $page = NULL) {
  function favorites_remove ($photo_id, $user_id = NULL) {
  function galleries_addPhoto ($gallery_id, $photo_id, $comment = NULL) {
  function galleries_create ($title, $description, $primary_photo_id = NULL) {
  function galleries_editMeta ($gallery_id, $title, $description = NULL) {
  function galleries_editPhoto ($gallery_id, $photo_id, $comment) {
  function galleries_editPhotos ($gallery_id, $primary_photo_id, $photo_ids) {
  function galleries_getInfo ($gallery_id) {
  function galleries_getList ($user_id, $per_page = NULL, $page = NULL) {
  function galleries_getListForPhoto ($photo_id, $per_page = NULL, $page = NULL) {
  function galleries_getPhotos ($gallery_id, $extras = NULL, $per_page = NULL, $page = NULL) {
  function groups_browse ($cat_id = NULL) {
  function groups_getInfo ($group_id, $lang = NULL) {
  function groups_search ($text, $per_page = NULL, $page = NULL) {
  function groups_members_getList ($group_id, $membertypes = NULL, $per_page = NULL, $page = NULL) {
  function groups_pools_add ($photo_id, $group_id) {
  function groups_pools_getContext ($photo_id, $group_id, $num_prev = NULL, $num_next = NULL) {
  function groups_pools_getGroups ($page = NULL, $per_page = NULL) {
  function groups_pools_getPhotos ($group_id, $tags = NULL, $user_id = NULL, $jump_to = NULL, $extras = NULL, $per_page = NULL, $page = NULL) {
  function groups_pools_remove ($photo_id, $group_id) {
  function interestingness_getList ($date = NULL, $use_panda = NULL, $extras = NULL, $per_page = NULL, $page = NULL) {
  function machinetags_getNamespaces ($predicate = NULL, $per_page = NULL, $page = NULL) {
  function machinetags_getPairs ($namespace = NULL, $predicate = NULL, $per_page = NULL, $page = NULL) {
  function machinetags_getPredicates ($namespace = NULL, $per_page = NULL, $page = NULL) {
  function machinetags_getRecentValues ($namespace = NULL, $predicate = NULL, $added_since = NULL) {
  function machinetags_getValues ($namespace, $predicate, $per_page = NULL, $page = NULL, $usage = NULL) {
  function panda_getList () {
  function panda_getPhotos ($panda_name, $extras = NULL, $per_page = NULL, $page = NULL) {
  function people_findByEmail ($find_email) {
  function people_findByUsername ($username) {
  function people_getInfo ($user_id) {
  function people_getPhotos ($user_id, $args = array()) {
  
  
  
  function people_getPhotosOf ($user_id, $extras = NULL, $per_page = NULL, $page = NULL) {
  function people_getPublicGroups ($user_id) {
  function people_getPublicPhotos ($user_id, $safe_search = NULL, $extras = NULL, $per_page = NULL, $page = NULL) {
  function people_getUploadStatus () {
  function photos_addTags ($photo_id, $tags) {
  function photos_delete ($photo_id) {
  function photos_getAllContexts ($photo_id) {
  function photos_getContactsPhotos ($count = NULL, $just_friends = NULL, $single_photo = NULL, $include_self = NULL, $extras = NULL) {
  function photos_getContactsPublicPhotos ($user_id, $count = NULL, $just_friends = NULL, $single_photo = NULL, $include_self = NULL, $extras = NULL) {
  function photos_getContext ($photo_id, $num_prev = NULL, $num_next = NULL, $extras = NULL, $order_by = NULL) {
  function photos_getCounts ($dates = NULL, $taken_dates = NULL) {
  function photos_getExif ($photo_id, $secret = NULL) {
  function photos_getFavorites ($photo_id, $page = NULL, $per_page = NULL) {
  function photos_getInfo ($photo_id, $secret = NULL, $humandates = NULL, $privacy_filter = NULL, $get_contexts = NULL) {
  function photos_getNotInSet ($max_upload_date = NULL, $min_taken_date = NULL, $max_taken_date = NULL, $privacy_filter = NULL, $media = NULL, $min_upload_date = NULL, $extras = NULL, $per_page = NULL, $page = NULL) {
  function photos_getPerms ($photo_id) {
  function photos_getRecent ($jump_to = NULL, $extras = NULL, $per_page = NULL, $page = NULL) {
  function photos_getSizes ($photo_id) {
  function photos_getUntagged ($min_upload_date = NULL, $max_upload_date = NULL, $min_taken_date = NULL, $max_taken_date = NULL, $privacy_filter = NULL, $media = NULL, $extras = NULL, $per_page = NULL, $page = NULL) {
  function photos_getWithGeoData ($args = array()) {
  
  
  function photos_getWithoutGeoData ($args = array()) {
  
  
  function photos_recentlyUpdated ($min_date, $extras = NULL, $per_page = NULL, $page = NULL) {
  function photos_removeTag ($tag_id) {
  function photos_search ($args = array()) {
  
  
  
  function photos_setContentType ($photo_id, $content_type) {
  function photos_setDates ($photo_id, $date_posted = NULL, $date_taken = NULL, $date_taken_granularity = NULL) {
  function photos_setMeta ($photo_id, $title, $description) {
  function photos_setPerms ($photo_id, $is_public, $is_friend, $is_family, $perm_comment, $perm_addmeta) {
  function photos_setSafetyLevel ($photo_id, $safety_level = NULL, $hidden = NULL) {
  function photos_setTags ($photo_id, $tags) {
  function photos_comments_addComment ($photo_id, $comment_text) {
  function photos_comments_deleteComment ($comment_id) {
  function photos_comments_editComment ($comment_id, $comment_text) {
  function photos_comments_getList ($photo_id, $min_comment_date = NULL, $max_comment_date = NULL, $page = NULL, $per_page = NULL, $include_faves = NULL) {
  function photos_comments_getRecentForContacts ($date_lastcomment = NULL, $contacts_filter = NULL, $extras = NULL, $per_page = NULL, $page = NULL) {
  function photos_geo_batchCorrectLocation ($lat, $lon, $accuracy, $place_id = NULL, $woe_id = NULL) {
  function photos_geo_correctLocation ($photo_id, $place_id = NULL, $woe_id = NULL) {
  function photos_geo_getLocation ($photo_id) {
  function photos_geo_getPerms ($photo_id) {
  function photos_geo_photosForLocation ($lat, $lon, $accuracy = NULL, $extras = NULL, $per_page = NULL, $page = NULL) {
  function photos_geo_removeLocation ($photo_id) {
  function photos_geo_setContext ($photo_id, $context) {
  function photos_geo_setLocation ($photo_id, $lat, $lon, $accuracy = NULL, $context = NULL, $bookmark_id = NULL) {
  function photos_geo_setPerms ($is_public, $is_contact, $is_friend, $is_family, $photo_id) {
  function photos_licenses_getInfo () {
  function photos_licenses_setLicense ($photo_id, $license_id) {
  function photos_notes_add ($photo_id, $note_x, $note_y, $note_w, $note_h, $note_text) {
  function photos_notes_delete ($note_id) {
  function photos_notes_edit ($note_id, $note_x, $note_y, $note_w, $note_h, $note_text) {
  function photos_transform_rotate ($photo_id, $degrees) {
  function photos_people_add ($photo_id, $user_id, $person_x = NULL, $person_y = NULL, $person_w = NULL, $person_h = NULL) {
  function photos_people_delete ($photo_id, $user_id, $email = NULL) {
  function photos_people_deleteCoords ($photo_id, $user_id) {
  function photos_people_editCoords ($photo_id, $user_id, $person_x, $person_y, $person_w, $person_h, $email = NULL) {
  function photos_people_getList ($photo_id) {
  function photos_upload_checkTickets ($tickets) {
  function photosets_addPhoto ($photoset_id, $photo_id) {
  function photosets_create ($title, $description, $primary_photo_id) {
  function photosets_delete ($photoset_id) {
  function photosets_editMeta ($photoset_id, $title, $description = NULL) {
  function photosets_editPhotos ($photoset_id, $primary_photo_id, $photo_ids) {
  function photosets_getContext ($photo_id, $photoset_id, $num_prev = NULL, $num_next = NULL) {
  function photosets_getInfo ($photoset_id) {
  function photosets_getList ($user_id = NULL, $page = NULL, $per_page = NULL, $primary_photo_extras = NULL) {
  function photosets_getPhotos ($photoset_id, $extras = NULL, $privacy_filter = NULL, $per_page = NULL, $page = NULL, $media = NULL) {
  function photosets_orderSets ($photoset_ids) {
  function photosets_removePhoto ($photoset_id, $photo_id) {
  function photosets_removePhotos ($photoset_id, $photo_ids) {
  function photosets_reorderPhotos ($photoset_id, $photo_ids) {
  function photosets_setPrimaryPhoto ($photoset_id, $photo_id) {
  function photosets_comments_addComment ($photoset_id, $comment_text) {
  function photosets_comments_deleteComment ($comment_id) {
  function photosets_comments_editComment ($comment_id, $comment_text) {
  function photosets_comments_getList ($photoset_id) {
  function places_find ($query) {
  function places_findByLatLon ($lat, $lon, $accuracy = NULL) {
  function places_getChildrenWithPhotosPublic ($place_id = NULL, $woe_id = NULL) {
  function places_getInfo ($place_id = NULL, $woe_id = NULL) {
  function places_getInfoByUrl ($url) {
  function places_getPlaceTypes () {
  function places_getShapeHistory ($place_id = NULL, $woe_id = NULL) {
  function places_getTopPlacesList ($place_type_id, $date = NULL, $woe_id = NULL, $place_id = NULL) {
  function places_placesForBoundingBox ($bbox, $place_type = NULL, $place_type_id = NULL, $recursive = NULL) {
  function places_placesForContacts ($place_type = NULL, $place_type_id = NULL, $woe_id = NULL, $place_id = NULL, $threshold = NULL, $contacts = NULL, $min_upload_date = NULL, $max_upload_date = NULL, $min_taken_date = NULL, $max_taken_date = NULL) {
  function places_placesForTags ($place_type_id, $woe_id = NULL, $place_id = NULL, $threshold = NULL, $tags = NULL, $tag_mode = NULL, $machine_tags = NULL, $machine_tag_mode = NULL, $min_upload_date = NULL, $max_upload_date = NULL, $min_taken_date = NULL, $max_taken_date = NULL) {
  function places_placesForUser ($place_type_id = NULL, $place_type = NULL, $woe_id = NULL, $place_id = NULL, $threshold = NULL, $min_upload_date = NULL, $max_upload_date = NULL, $min_taken_date = NULL, $max_taken_date = NULL) {
  function places_resolvePlaceId ($place_id) {
  function places_resolvePlaceURL ($url) {
  function places_tagsForPlace ($woe_id = NULL, $place_id = NULL, $min_upload_date = NULL, $max_upload_date = NULL, $min_taken_date = NULL, $max_taken_date = NULL) {
  function prefs_getContentType () {
  function prefs_getGeoPerms () {
  function prefs_getHidden () {
  function prefs_getPrivacy () {
  function prefs_getSafetyLevel () {
  function reflection_getMethodInfo ($method_name) {
  function reflection_getMethods () {
  function stats_getCollectionDomains ($date, $collection_id = NULL, $per_page = NULL, $page = NULL) {
  function stats_getCollectionReferrers ($date, $domain, $collection_id = NULL, $per_page = NULL, $page = NULL) {
  function stats_getCollectionStats ($date, $collection_id) {
  function stats_getCSVFiles () {
  function stats_getPhotoDomains ($date, $photo_id = NULL, $per_page = NULL, $page = NULL) {
  function stats_getPhotoReferrers ($date, $domain, $photo_id = NULL, $per_page = NULL, $page = NULL) {
  function stats_getPhotosetDomains ($date, $photoset_id = NULL, $per_page = NULL, $page = NULL) {
  function stats_getPhotosetReferrers ($date, $domain, $photoset_id = NULL, $per_page = NULL, $page = NULL) {
  function stats_getPhotosetStats ($date, $photoset_id) {
  function stats_getPhotoStats ($date, $photo_id) {
  function stats_getPhotostreamDomains ($date, $per_page = NULL, $page = NULL) {
  function stats_getPhotostreamReferrers ($date, $domain, $per_page = NULL, $page = NULL) {
  function stats_getPhotostreamStats ($date) {
  function stats_getPopularPhotos ($date = NULL, $sort = NULL, $per_page = NULL, $page = NULL) {
  function stats_getTotalViews ($date = NULL) {
  function tags_getClusterPhotos ($tag, $cluster_id) {
  function tags_getClusters ($tag) {
  function tags_getHotList ($period = NULL, $count = NULL) {
  function tags_getListPhoto ($photo_id) {
  function tags_getListUser ($user_id = NULL) {
  function tags_getListUserPopular ($user_id = NULL, $count = NULL) {
  function tags_getListUserRaw ($tag = NULL) {
  function tags_getRelated ($tag) {
  function test_echo ($args = array()) {
  function test_login () {
  function urls_getGroup ($group_id) {
  function urls_getUserPhotos ($user_id = NULL) {
  function urls_getUserProfile ($user_id = NULL) {
  function urls_lookupGallery ($url) {
  function urls_lookupGroup ($url) {
  function urls_lookupUser ($url) {
}
//end class
Class phpFlickr_pager {
  function phpFlickr_pager($phpFlickr, $method = null, $args = null, $per_page = 30) {
  function set_phpFlickr($phpFlickr) {
  function __sleep() {
  function load($page) {
  function get($page = null) {
  function next() {
