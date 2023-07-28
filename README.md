# p2l-translations

translations and messages for the p2l menu

## configuration

when instantiating translation service, set members to the following settings:

```cpp
namespace p2l
{
	translation_service::translation_service() :
	    m_url("https://raw.githubusercontent.com/sinjs/p2l-translations/main"),
	    m_fallback_url("https://cdn.pene.cc/p2l-translations/main/")
	{}

	// ...
```

where `m_fallback_url` is a mirror, or fallback version of the translation, incase github goes
down or the translation is not availible for any other reason. if there is no fallback url
availible, use the same url as the main url to skip fallback checking. in this case the example
is hosted on the pene cdn at `https://cdn.pene.cc/p2l-translations/main`
