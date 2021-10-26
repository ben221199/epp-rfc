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
	<svID/>		<!--[REQUIRED] Server ID: The name of the server-->
	<svDate/>	<!--[REQUIRED] Server Date-->
	<svcMenu>	<!--[REQUIRED] Service Menu-->
		<version/>	<!--[1-*] Version: Protocol versions supported by the server-->
		<lang/>		<!--[1-*] Language: Languages supported by the server-->
		<objURI/>	<!--[1-*] Object URI: URIs of the objects managed by the server-->
		<svcExtension>	<!--[OPTIONAL] Service Extension-->
			<extURI/>	<!--[1-*] Extension URI: URIs of the extension objects managed by the server-->
		</svcExtension>
	</svcMenu>
	<dcp>		<!--[REQUIRED] Data Collection Policy-->
		<access>	<!--[REQUIRED] Access: The access mode of the current client-->
			<all/>		<!--[0-1] All-->
			<!--OR-->
			<none/>		<!--[0-1] None-->
			<!--OR-->
			<null/>		<!--[0-1] Null-->
			<!--OR-->
			<personal/>	<!--[0-1] Personal-->
			<!--OR-->
			<personalAndOther/><!--[0-1] Personal And Other-->
			<!--OR-->
			<other/>	<!--[0-1] Other-->
		</access>
		<statement>	<!--[1-*] Statement-->
			<purpose>	<!--[REQUIRED] Purpose-->
				<admin/>	<!--[0-*] Admin-->
				<!--AND/OR-->
				<contact/>	<!--[0-*] Contact-->
				<!--AND/OR-->
				<prov/>		<!--[0-*] Provisioning-->
				<!--AND/OR-->
				<other/>	<!--[0-*] Other-->
			</purpose>
			<recipient>	<!--[REQUIRED] Recipient-->
				<other/>	<!--[0-*] Other-->
				<!--AND/OR-->
				<ours>		<!--[0-*] Ours-->
					<recDesc/>	<!--[OPTIONAL] Recipient Description-->
				</ours>
				<!--AND/OR-->
				<public/>	<!--[0-*] Public-->
				<!--AND/OR-->
				<same/>		<!--[0-*] Same-->
				<!--AND/OR-->
				<unrelated/>	<!--[0-*] Unrelated-->
			</recipient>
			<retention>	<!--[REQUIRED] Retention-->
				<business/>	<!--[0-1] Business-->
				<!--OR-->
				<indefinite/>	<!--[0-1] Indefinite-->
				<!--OR-->
				<legal/>	<!--[0-1] Legal-->
				<!--OR-->
				<none/>		<!--[0-1] None-->
				<!--OR-->
				<stated/>	<!--[0-1] Stated-->
			</retention>
		</<statement>
		<expiry>	<!--[OPTIONAL] Expiry-->
			<absolute/>	<!--[0-1] Absolute-->
			<!--OR-->
			<relative/>	<!--[0-1] Relaive-->
		</expiry>
	</dcp>
</greeting>
```

## Format: Command

```xml
<command>
	<!--$COMMAND-->
</command>
```

### Command: Login (Session Management)

```xml
<login>
	<!--$LOGIN-->
</login>
```

### Command: Logout (Session Management)

```xml
<logout/>
```

### Command: Check (Query)

```xml
<check>
	<!--$CHECK-->
</check>
```

### Command: Info (Query)

```xml
<info>
	<!--$INFO-->
</info>
```

### Command: Poll (Query)

```xml
<poll op="ack|req" msgId="optional:message_id">
	<!--$POLL-->
</poll>
```

### Command: Transfer (Query)

```xml
<transfer op="query">
	<!--$TRANSFER-->
</transfer>
```

### Command: Create (Object Transform)

```xml
<create>
	<!--$CREATE-->
</create>
```

### Command: Delete (Object Transform)

```xml
<delete>
	<!--$DELETE-->
</delete>
```

### Command: Renew (Object Transform)

```xml
<renew>
	<!--$RENEW-->
</renew>
```

### Command: Transfer (Object Transform)

```xml
<transfer op="approve|cancel|query|reject|request">
	<!--$TRANSFER-->
</transfer>
```

### Command: Update (Object Transform)

```xml
<update>
	<!--$UPDATE-->
</update>
```

## Format: Response

```xml
<response>
	<!--$RESPONSE-->
</response>
```
