# *Add to the subtheme.libraries.yml*

#Half and Half <br />
half_and_half: <br />
version: "1.0.x" <br />
css: <br />
theme: <br />
//cdnjs.cloudflare.com/ajax/libs/animate.css/4.1.1/animate.min.css: { type: external } <br />
templates/block/custom/half_and_half/css/half_and_half.css: {} <br />
js: <br />
//cdnjs.cloudflare.com/ajax/libs/waypoints/4.0.1/jquery.waypoints.min.js: { type: external } <br />
templates/block/custom/half_and_half/js/waypoint.js: {} <br />
dependencies: <br />
- core/jquery <br />

# *Add to the repositories section in subtheme composer.json*

"repositories": [ <br />
{ <br />
"type": "vcs", <br />
"url": "https://github.gatech.edu/ICWebTeam/block_half_and_half.git" <br />
}
# *Add to the require in subtheme composer.json*

"require": { <br />
"gt/half_and_half": "dev-master" <br />
"mnsami/composer-custom-directory-installer": "^2.0"<br />
},

# *Add to the installer paths in subtheme composer.json*
"installer-paths": { <br />
"web/themes/custom/SUBTHEME/templates/block/custom/half_and_half": [ <br />
"gt/half_and_half" <br />
] <br />
},

# *Implements hook_page_attachments_alter(). in subtheme.theme*
function tlw_page_attachments_alter(&$page) {<br />
$page['#attached']['library'][] = 'SUBTHEME/half_and_half';<br />
}


# **TAXONOMY SET-UP**
![](images/animations.png)
