# 变量
## settings
{{ settings.logo_width }} 指变量在 config/settings_data.json

## section
{{ section.settings.width1  }} 变量为当前 liquid
{% schema %}
{
  "name": "t:sections.main-password-header.name",
  "settings": [
    {
      "type": "text",
      "id": "width1",
      "label": "宽度1",
      "default": "100px"
    },
  ]
}
{% endschema %}
type	设置类型，可以是任何基本或专用输入设置类型。	是的
id	设置ID，用于访问设置值。	是的
label	设置标签，将显示在主题编辑器中。	是的
default	设置的默认值。	不
info	有关设置的信息文本选项。	不

## shop
{{ shop.id }}
{{ shop.name }}
{{ shop.moneyFormat }}

## request
{{ request.locale }}
{{ request.path }}


# 渲染子节点

## render
{%- render 'icon-facebook' -%}
snippets/icon-facebook.liquid

## sections
{% sections 'header-group' %}
sections/header-group.json
announcement-bar.liquid
header.liquid

{% sections 'footer-group' %}
sections/footer-group.json
footer.liquid


# 判断为空
blank
{%- if settings.social_twitter_link != blank -%}
<span>111</span>
{%- endif -%}

# 多语言
{{ 'general.social.links.snapchat' | t }}

# 过滤器
1.  如何创建一个过滤器


