# Non-responsive Theme
### An example for Liferay 6.2 non-responsive theme.

Liferay 6.2 themes have by default responsive capabilities. Sometimes, mainly for legacy purposes, it is required to disable this functionality. You can disable the responsive features by createing a new custome theme that will overwrite the responsive code.

## What need to be done:
* Create a empty new theme. Set parent to _styled.
* Add files that needs to be modified
	* css/dockbar.css
	* css/aui/responsive.scss
	* templates/portal_normal.vm
* Comment out the _@media_ query in dockbar.css.
* Comment out the content of responsive.scss.
* Add fix viewport to the portal_normal template.
