flickr document

https://www.flickr.com/services/api/auth.howto.web.html\

https://www.flickr.com/services/api/auth.oauth.html

![alt tag](https://raw.githubusercontent.com/0way/phpflickr/master/hinh_mieuta.png)

List Class and funtion important in  phpFlickr.php


class phpFlickr { <br />

function phpFlickr ($api_key, $secret = NULL, $die_on_error = false) { <br />
function enableCache ($type, $connection, $cache_expire = 600, $table = 'flickr_cache') { <br />
function getCached ($request)
function cache ($request, $response)
function setCustomPost ( $function ) { <br />
function setCustomPost ( $function ) { <br />

function post ($data, $type = null) { <br />

function request ($command, $args = array(), $nocache = false)
function clean_text_nodes ($arr) { <br />
function setToken ($token) { <br />
function setProxy ($server, $port) { <br />
function getErrorCode () { <br />
function getErrorMsg () { <br />
function buildPhotoURL ($photo, $size = "Medium") { <br />
function sync_upload ($photo, $title = null, $description = null, $tags = null, $is_public = null, $is_friend = null, $is_family = null) { <br />

function async_upload ($photo, $title = null, $description = null, $tags = null, $is_public = null, $is_friend = null, $is_family = null) { <br />

function replace ($photo, $photo_id, $async = null) { <br />

function auth ($perms = "read", $remember_uri = true) { <br />
function auth_url($frob, $perms = 'read') { <br />
function call ($method, $arguments) { <br />


function activity_userComments ($per_page = NULL, $page = NULL) { <br />
function activity_userPhotos ($timeframe = NULL, $per_page = NULL, $page = NULL) { <br />
function auth_checkToken () { <br />
function auth_getFrob () { <br />
function auth_getFullToken ($mini_token) { <br />
function auth_getToken ($frob) { <br />
function blogs_getList ($service = NULL) { <br />
function blogs_getServices () { <br />
function blogs_postPhoto ($blog_id = NULL, $photo_id, $title, $description, $blog_password = NULL, $service = NULL) { <br />
function collections_getInfo ($collection_id) { <br />
function collections_getTree ($collection_id = NULL, $user_id = NULL) { <br />
function commons_getInstitutions () { <br />
function contacts_getList ($filter = NULL, $page = NULL, $per_page = NULL) { <br />
function contacts_getPublicList ($user_id, $page = NULL, $per_page = NULL) { <br />
function contacts_getListRecentlyUploaded ($date_lastupload = NULL, $filter = NULL) { <br />
function favorites_add ($photo_id) { <br />
function favorites_getList ($user_id = NULL, $jump_to = NULL, $min_fave_date = NULL, $max_fave_date = NULL, $extras = NULL, $per_page = NULL, $page = NULL) { <br />
function favorites_getPublicList ($user_id, $jump_to = NULL, $min_fave_date = NULL, $max_fave_date = NULL, $extras = NULL, $per_page = NULL, $page = NULL) { <br />
function favorites_remove ($photo_id, $user_id = NULL) { <br />
function galleries_addPhoto ($gallery_id, $photo_id, $comment = NULL) { <br />
function galleries_create ($title, $description, $primary_photo_id = NULL) { <br />
function galleries_editMeta ($gallery_id, $title, $description = NULL) { <br />
function galleries_editPhoto ($gallery_id, $photo_id, $comment) { <br />
function galleries_editPhotos ($gallery_id, $primary_photo_id, $photo_ids) { <br />
function galleries_getInfo ($gallery_id) { <br />
function galleries_getList ($user_id, $per_page = NULL, $page = NULL) { <br />
function galleries_getListForPhoto ($photo_id, $per_page = NULL, $page = NULL) { <br />
function galleries_getPhotos ($gallery_id, $extras = NULL, $per_page = NULL, $page = NULL) { <br />
function groups_browse ($cat_id = NULL) { <br />
function groups_getInfo ($group_id, $lang = NULL) { <br />
function groups_search ($text, $per_page = NULL, $page = NULL) { <br />
function groups_members_getList ($group_id, $membertypes = NULL, $per_page = NULL, $page = NULL) { <br />
function groups_pools_add ($photo_id, $group_id) { <br />
function groups_pools_getContext ($photo_id, $group_id, $num_prev = NULL, $num_next = NULL) { <br />
function groups_pools_getGroups ($page = NULL, $per_page = NULL) { <br />
function groups_pools_getPhotos ($group_id, $tags = NULL, $user_id = NULL, $jump_to = NULL, $extras = NULL, $per_page = NULL, $page = NULL) { <br />
function groups_pools_remove ($photo_id, $group_id) { <br />
function interestingness_getList ($date = NULL, $use_panda = NULL, $extras = NULL, $per_page = NULL, $page = NULL) { <br />
function machinetags_getNamespaces ($predicate = NULL, $per_page = NULL, $page = NULL) { <br />
function machinetags_getPairs ($namespace = NULL, $predicate = NULL, $per_page = NULL, $page = NULL) { <br />
function machinetags_getPredicates ($namespace = NULL, $per_page = NULL, $page = NULL) { <br />
function machinetags_getRecentValues ($namespace = NULL, $predicate = NULL, $added_since = NULL) { <br />
function machinetags_getValues ($namespace, $predicate, $per_page = NULL, $page = NULL, $usage = NULL) { <br />
function panda_getList () { <br />
function panda_getPhotos ($panda_name, $extras = NULL, $per_page = NULL, $page = NULL) { <br />
function people_findByEmail ($find_email) { <br />
function people_findByUsername ($username) { <br />
function people_getInfo ($user_id) { <br />
function people_getPhotos ($user_id, $args = array()) { <br />



function people_getPhotosOf ($user_id, $extras = NULL, $per_page = NULL, $page = NULL) { <br />
function people_getPublicGroups ($user_id) { <br />
function people_getPublicPhotos ($user_id, $safe_search = NULL, $extras = NULL, $per_page = NULL, $page = NULL) { <br />
function people_getUploadStatus () { <br />
function photos_addTags ($photo_id, $tags) { <br />
function photos_delete ($photo_id) { <br />
function photos_getAllContexts ($photo_id) { <br />
function photos_getContactsPhotos ($count = NULL, $just_friends = NULL, $single_photo = NULL, $include_self = NULL, $extras = NULL) { <br />
function photos_getContactsPublicPhotos ($user_id, $count = NULL, $just_friends = NULL, $single_photo = NULL, $include_self = NULL, $extras = NULL) { <br />
function photos_getContext ($photo_id, $num_prev = NULL, $num_next = NULL, $extras = NULL, $order_by = NULL) { <br />
function photos_getCounts ($dates = NULL, $taken_dates = NULL) { <br />
function photos_getExif ($photo_id, $secret = NULL) { <br />
function photos_getFavorites ($photo_id, $page = NULL, $per_page = NULL) { <br />
function photos_getInfo ($photo_id, $secret = NULL, $humandates = NULL, $privacy_filter = NULL, $get_contexts = NULL) { <br />
function photos_getNotInSet ($max_upload_date = NULL, $min_taken_date = NULL, $max_taken_date = NULL, $privacy_filter = NULL, $media = NULL, $min_upload_date = NULL, $extras = NULL, $per_page = NULL, $page = NULL) { <br />
function photos_getPerms ($photo_id) { <br />
function photos_getRecent ($jump_to = NULL, $extras = NULL, $per_page = NULL, $page = NULL) { <br />
function photos_getSizes ($photo_id) { <br />
function photos_getUntagged ($min_upload_date = NULL, $max_upload_date = NULL, $min_taken_date = NULL, $max_taken_date = NULL, $privacy_filter = NULL, $media = NULL, $extras = NULL, $per_page = NULL, $page = NULL) { <br />
function photos_getWithGeoData ($args = array()) { <br />


function photos_getWithoutGeoData ($args = array()) { <br />


function photos_recentlyUpdated ($min_date, $extras = NULL, $per_page = NULL, $page = NULL) { <br />
function photos_removeTag ($tag_id) { <br />
function photos_search ($args = array()) { <br />



function photos_setContentType ($photo_id, $content_type) { <br />
function photos_setDates ($photo_id, $date_posted = NULL, $date_taken = NULL, $date_taken_granularity = NULL) { <br />
function photos_setMeta ($photo_id, $title, $description) { <br />
function photos_setPerms ($photo_id, $is_public, $is_friend, $is_family, $perm_comment, $perm_addmeta) { <br />
function photos_setSafetyLevel ($photo_id, $safety_level = NULL, $hidden = NULL) { <br />
function photos_setTags ($photo_id, $tags) { <br />
function photos_comments_addComment ($photo_id, $comment_text) { <br />
function photos_comments_deleteComment ($comment_id) { <br />
function photos_comments_editComment ($comment_id, $comment_text) { <br />
function photos_comments_getList ($photo_id, $min_comment_date = NULL, $max_comment_date = NULL, $page = NULL, $per_page = NULL, $include_faves = NULL) { <br />
function photos_comments_getRecentForContacts ($date_lastcomment = NULL, $contacts_filter = NULL, $extras = NULL, $per_page = NULL, $page = NULL) { <br />
function photos_geo_batchCorrectLocation ($lat, $lon, $accuracy, $place_id = NULL, $woe_id = NULL) { <br />
function photos_geo_correctLocation ($photo_id, $place_id = NULL, $woe_id = NULL) { <br />
function photos_geo_getLocation ($photo_id) { <br />
function photos_geo_getPerms ($photo_id) { <br />
function photos_geo_photosForLocation ($lat, $lon, $accuracy = NULL, $extras = NULL, $per_page = NULL, $page = NULL) { <br />
function photos_geo_removeLocation ($photo_id) { <br />
function photos_geo_setContext ($photo_id, $context) { <br />
function photos_geo_setLocation ($photo_id, $lat, $lon, $accuracy = NULL, $context = NULL, $bookmark_id = NULL) { <br />
function photos_geo_setPerms ($is_public, $is_contact, $is_friend, $is_family, $photo_id) { <br />
function photos_licenses_getInfo () { <br />
function photos_licenses_setLicense ($photo_id, $license_id) { <br />
function photos_notes_add ($photo_id, $note_x, $note_y, $note_w, $note_h, $note_text) { <br />
function photos_notes_delete ($note_id) { <br />
function photos_notes_edit ($note_id, $note_x, $note_y, $note_w, $note_h, $note_text) { <br />
function photos_transform_rotate ($photo_id, $degrees) { <br />
function photos_people_add ($photo_id, $user_id, $person_x = NULL, $person_y = NULL, $person_w = NULL, $person_h = NULL) { <br />
function photos_people_delete ($photo_id, $user_id, $email = NULL) { <br />
function photos_people_deleteCoords ($photo_id, $user_id) { <br />
function photos_people_editCoords ($photo_id, $user_id, $person_x, $person_y, $person_w, $person_h, $email = NULL) { <br />
function photos_people_getList ($photo_id) { <br />
function photos_upload_checkTickets ($tickets) { <br />
function photosets_addPhoto ($photoset_id, $photo_id) { <br />
function photosets_create ($title, $description, $primary_photo_id) { <br />
function photosets_delete ($photoset_id) { <br />
function photosets_editMeta ($photoset_id, $title, $description = NULL) { <br />
function photosets_editPhotos ($photoset_id, $primary_photo_id, $photo_ids) { <br />
function photosets_getContext ($photo_id, $photoset_id, $num_prev = NULL, $num_next = NULL) { <br />
function photosets_getInfo ($photoset_id) { <br />
function photosets_getList ($user_id = NULL, $page = NULL, $per_page = NULL, $primary_photo_extras = NULL) { <br />
function photosets_getPhotos ($photoset_id, $extras = NULL, $privacy_filter = NULL, $per_page = NULL, $page = NULL, $media = NULL) { <br />
function photosets_orderSets ($photoset_ids) { <br />
function photosets_removePhoto ($photoset_id, $photo_id) { <br />
function photosets_removePhotos ($photoset_id, $photo_ids) { <br />
function photosets_reorderPhotos ($photoset_id, $photo_ids) { <br />
function photosets_setPrimaryPhoto ($photoset_id, $photo_id) { <br />
function photosets_comments_addComment ($photoset_id, $comment_text) { <br />
function photosets_comments_deleteComment ($comment_id) { <br />
function photosets_comments_editComment ($comment_id, $comment_text) { <br />
function photosets_comments_getList ($photoset_id) { <br />
function places_find ($query) { <br />
function places_findByLatLon ($lat, $lon, $accuracy = NULL) { <br />
function places_getChildrenWithPhotosPublic ($place_id = NULL, $woe_id = NULL) { <br />
function places_getInfo ($place_id = NULL, $woe_id = NULL) { <br />
function places_getInfoByUrl ($url) { <br />
function places_getPlaceTypes () { <br />
function places_getShapeHistory ($place_id = NULL, $woe_id = NULL) { <br />
function places_getTopPlacesList ($place_type_id, $date = NULL, $woe_id = NULL, $place_id = NULL) { <br />
function places_placesForBoundingBox ($bbox, $place_type = NULL, $place_type_id = NULL, $recursive = NULL) { <br />
function places_placesForContacts ($place_type = NULL, $place_type_id = NULL, $woe_id = NULL, $place_id = NULL, $threshold = NULL, $contacts = NULL, $min_upload_date = NULL, $max_upload_date = NULL, $min_taken_date = NULL, $max_taken_date = NULL) { <br />
function places_placesForTags ($place_type_id, $woe_id = NULL, $place_id = NULL, $threshold = NULL, $tags = NULL, $tag_mode = NULL, $machine_tags = NULL, $machine_tag_mode = NULL, $min_upload_date = NULL, $max_upload_date = NULL, $min_taken_date = NULL, $max_taken_date = NULL) { <br />
function places_placesForUser ($place_type_id = NULL, $place_type = NULL, $woe_id = NULL, $place_id = NULL, $threshold = NULL, $min_upload_date = NULL, $max_upload_date = NULL, $min_taken_date = NULL, $max_taken_date = NULL) { <br />
function places_resolvePlaceId ($place_id) { <br />
function places_resolvePlaceURL ($url) { <br />
function places_tagsForPlace ($woe_id = NULL, $place_id = NULL, $min_upload_date = NULL, $max_upload_date = NULL, $min_taken_date = NULL, $max_taken_date = NULL) { <br />
function prefs_getContentType () { <br />
function prefs_getGeoPerms () { <br />
function prefs_getHidden () { <br />
function prefs_getPrivacy () { <br />
function prefs_getSafetyLevel () { <br />
function reflection_getMethodInfo ($method_name) { <br />
function reflection_getMethods () { <br />
function stats_getCollectionDomains ($date, $collection_id = NULL, $per_page = NULL, $page = NULL) { <br />
function stats_getCollectionReferrers ($date, $domain, $collection_id = NULL, $per_page = NULL, $page = NULL) { <br />
function stats_getCollectionStats ($date, $collection_id) { <br />
function stats_getCSVFiles () { <br />
function stats_getPhotoDomains ($date, $photo_id = NULL, $per_page = NULL, $page = NULL) { <br />
function stats_getPhotoReferrers ($date, $domain, $photo_id = NULL, $per_page = NULL, $page = NULL) { <br />
function stats_getPhotosetDomains ($date, $photoset_id = NULL, $per_page = NULL, $page = NULL) { <br />
function stats_getPhotosetReferrers ($date, $domain, $photoset_id = NULL, $per_page = NULL, $page = NULL) { <br />
function stats_getPhotosetStats ($date, $photoset_id) { <br />
function stats_getPhotoStats ($date, $photo_id) { <br />
function stats_getPhotostreamDomains ($date, $per_page = NULL, $page = NULL) { <br />
function stats_getPhotostreamReferrers ($date, $domain, $per_page = NULL, $page = NULL) { <br />
function stats_getPhotostreamStats ($date) { <br />
function stats_getPopularPhotos ($date = NULL, $sort = NULL, $per_page = NULL, $page = NULL) { <br />
function stats_getTotalViews ($date = NULL) { <br />
function tags_getClusterPhotos ($tag, $cluster_id) { <br />
function tags_getClusters ($tag) { <br />
function tags_getHotList ($period = NULL, $count = NULL) { <br />
function tags_getListPhoto ($photo_id) { <br />
function tags_getListUser ($user_id = NULL) { <br />
function tags_getListUserPopular ($user_id = NULL, $count = NULL) { <br />
function tags_getListUserRaw ($tag = NULL) { <br />
function tags_getRelated ($tag) { <br />
function test_echo ($args = array()) { <br />
function test_login () { <br />
function urls_getGroup ($group_id) { <br />
function urls_getUserPhotos ($user_id = NULL) { <br />
function urls_getUserProfile ($user_id = NULL) { <br />
function urls_lookupGallery ($url) { <br />
function urls_lookupGroup ($url) { <br />
function urls_lookupUser ($url) { <br />
}
//end class





Class phpFlickr_pager { <br />
function phpFlickr_pager($phpFlickr, $method = null, $args = null, $per_page = 30) { <br />
function set_phpFlickr($phpFlickr) { <br />
function __sleep() { <br />
function load($page) { <br />
function get($page = null) { <br />
function next() { <br />

