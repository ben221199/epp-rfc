# EPP

```xml
<epp
	xmlns="urn:ietf:params:xml:ns:epp-1.0"
	xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
	xsi:schemaLocation="urn:ietf:params:xml:ns:epp-1.0 epp-1.0.xsd">
	<!--$FORMAT-->
</epp>
```

## Format: Hello

```xml
<hello/>
```

## Format: Greeting

```xml
<greeting>
	<svID/>		<!--Server ID: The name of the server-->
	<svDate/>	<!--Server Date-->
	<svcMenu>	<!--Service Menu-->
		<version/>	<!--[1-*] Version: Protocol versions supported by the server-->
		<lang/>		<!--[1-*] Language: Languages supported by the server-->
		<objURI/>	<!--[1-*] Object URI: URIs of the objects managed by the server-->
		<svcExtension>	<!--[OPTIONAL] Service Extension-->
			<extURI/>	<!--[1-*] Extension URI: URIs of the extension objects managed by the server-->
		</svcExtension>
	</svcMenu>
	<dcp>		<!--Data Collection Policy-->
		<access>	<!--Access: The access mode of the current client-->
			<all/>		<!--All-->
			<!--OR-->
			<none/>		<!--None-->
			<!--OR-->
			<null/>		<!--Null-->
			<!--OR-->
			<personal/>	<!--Personal-->
			<!--OR-->
			<personalAndOther/><!--Personal And Other-->
			<!--OR-->
			<other/>	<!--Other-->
		</access>
	</dcp>
</greeting>
```

## Format: Command

```xml
<command>
	<!--$COMMAND-->
</command>

## Format: Response

```xml
<command>
	<!--$RESPONSE-->
</command>
