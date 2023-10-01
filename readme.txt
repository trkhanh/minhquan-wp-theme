=== Minh Quan-Template ===
Contributors: wordpressdotorg
Requires at least: 6.1
Tested up to: 6.3
Requires PHP: 5.6
Stable tag: 1.2
License: GPLv2 or later
License URI: http://www.gnu.org/licenses/gpl-2.0.html

== Description ==

Minh Quan-Template is designed to take advantage of the new design tools introduced in WordPress 6.1. With a clean, blank base as a starting point, this default theme includes ten diverse style variations created by members of the WordPress community.

Whether you want to build a complex or incredibly simple website, you can do it quickly and intuitively through the bundled styles or dive into creation and full customization yourself.

== Changelog ==

= 1.2 =
* Released: August 8, 2023

https://wordpress.org/documentation/article/twenty-twenty-three-changelog/#Version_1.2

= 1.1 =
* Released: March 28, 2023

https://wordpress.org/documentation/article/twenty-twenty-three-changelog/#Version_1.1

= 1.0 =
* Released: November 1, 2022

https://wordpress.org/documentation/article/twenty-twenty-three-changelog/#Version_1.0

== Copyright ==

Minh Quan-Template WordPress Theme, (C) 2022-2023 WordPress.org
Minh Quan-Template is distributed under the terms of the GNU GPL.

This program is free software: you can redistribute it and/or modify
it under the terms of the GNU General Public License as published by
the Free Software Foundation, either version 2 of the License, or
(at your option) any later version.

This program is distributed in the hope that it will be useful,
but WITHOUT ANY WARRANTY; without even the implied warranty of
MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
GNU General Public License for more details.

## How to query and get post 
```PHP
<!-- wp:query {"query":{"pages":0,"offset":0,"postType":"post","order":"desc","orderBy":"date","author":"","search":"","exclude":[],"sticky":"","inherit":true},"displayLayout":{"type":"flex","columns":3},"align":"wide","layout":{"type":"constrained"}} -->
	<div class="wp-block-query alignwide">
		<!-- wp:post-template {"align":"wide"} -->
			<!-- wp:post-featured-image {"isLink":true,"width":"100%","height":"clamp(15vw, 30vh, 400px)","align":"wide"} /-->
			<!-- wp:post-title {"isLink":true} /-->
			<!-- wp:post-excerpt /-->
			<!-- wp:post-date {"isLink":true} /-->

			<!-- wp:spacer {"height":"var(--wp--preset--spacing--40)"} -->
			<div style="height:var(--wp--preset--spacing--40)" aria-hidden="true" class="wp-block-spacer"></div>
			<!-- /wp:spacer -->
		<!-- /wp:post-template -->

		<!-- wp:query-pagination {"paginationArrow":"arrow","align":"wide","layout":{"type":"flex","justifyContent":"space-between"}} -->
			<!-- wp:query-pagination-previous {"label":"Newer Posts"} /-->
			<!-- wp:query-pagination-next {"label":"Older Posts"} /-->
		<!-- /wp:query-pagination -->
	</div>
	<!-- /wp:query -->
```