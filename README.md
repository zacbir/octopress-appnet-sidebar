octopress-appnet-sidebar
========================

App.net Sidebar for Octopress

Using it involves three steps:

1. [Adding the Files](#step-1)
2. [Stitching up the Local Sass Rules](#step-2)
3. [Configuring your App.net Variables](#step-3)

## <a name="step-1"></a>Adding the Files

### Template

`source/_includes/custom/asides/adn.html`

### Javascript

`source/javascripts/adn.js`

### Sass

`sass/partials/sidebar/_adn.scss`

### Images

`source/images/adn_32_gray.png`

## <a name="step-2"></a>Stitching up the Local Sass Rules

Beyond simple dropping the above files in the correct place, you'll need to edit the following
file to include the ADN Sass for compilation:

`sass/partials/_sidebar.scss`

{% codeblock lang:sass %}
@import "sidebar/adn";
{% endcodeblock %}

## <a name="step-3"></a>Configuring your App.net Variables

Configuration is simple. Just add some variables to your `_config.yaml` file:

    # App.net
    adn_user: urbanape
    adn_post_count: 5
    adn_show_replies: false
