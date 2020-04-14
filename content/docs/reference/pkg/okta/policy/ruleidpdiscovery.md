
---
title: "RuleIdpDiscovery"
block_external_search_index: true
---



Creates an IdP Discovery Policy Rule.

This resource allows you to create and configure an IdP Discovery Policy Rule.

## Example Usage

```typescript
import * as pulumi from "@pulumi/pulumi";
import * as okta from "@pulumi/okta";

const example = new okta.policy.RuleIdpDiscovery("example", {
    idpId: "<idp id>",
    idpType: "SAML2",
    policyid: "<policy id>",
    priority: 1,
    userIdentifierAttribute: "company",
    userIdentifierPatterns: [{
        matchType: "EQUALS",
        value: "Articulate",
    }],
    userIdentifierType: "ATTRIBUTE",
});
```

> This content is derived from https://github.com/articulate/terraform-provider-okta/blob/master/website/docs/r/policy_rule_idp_discovery.html.markdown.



## Create a RuleIdpDiscovery Resource

{{< chooser language "javascript,typescript,python,go,csharp" / >}}

{{% choosable language nodejs %}}
<div class="highlight"><pre class="chroma"><code class="language-typescript" data-lang="typescript"><span class="k">new </span><span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/okta/policy/#RuleIdpDiscovery">RuleIdpDiscovery</a></span><span class="p">(</span><span class="nx">name</span>: <span class="nx"><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string">string</a></span><span class="p">, </span><span class="nx">args</span>: <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/okta/policy/#RuleIdpDiscoveryArgs">RuleIdpDiscoveryArgs</a></span><span class="p">, </span><span class="nx">opts</span>?: <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/pulumi/#CustomResourceOptions">pulumi.CustomResourceOptions</a></span><span class="p">);</span></code></pre></div>
{{% /choosable %}}

{{% choosable language python %}}
<div class="highlight"><pre class="chroma"><code class="language-python" data-lang="python"><span class="k">def </span><span class="nf">RuleIdpDiscovery</span><span class="p">(resource_name, opts=None, </span>app_excludes=None<span class="p">, </span>app_includes=None<span class="p">, </span>idp_id=None<span class="p">, </span>idp_type=None<span class="p">, </span>name=None<span class="p">, </span>network_connection=None<span class="p">, </span>network_excludes=None<span class="p">, </span>network_includes=None<span class="p">, </span>platform_includes=None<span class="p">, </span>policyid=None<span class="p">, </span>priority=None<span class="p">, </span>status=None<span class="p">, </span>user_identifier_attribute=None<span class="p">, </span>user_identifier_patterns=None<span class="p">, </span>user_identifier_type=None<span class="p">, __props__=None);</span></code></pre></div>
{{% /choosable %}}

{{% choosable language go %}}
<div class="highlight"><pre class="chroma"><code class="language-go" data-lang="go"><span class="k">func </span>NewRuleIdpDiscovery<span class="p">(</span><span class="nx">ctx</span> *<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#Context">pulumi.Context</a></span><span class="p">, </span><span class="nx">name</span> <span class="nx"><a href="https://golang.org/pkg/builtin/#string">string</a></span><span class="p">, </span><span class="nx">args</span> <span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi-okta/sdk/go/okta/policy?tab=doc#RuleIdpDiscoveryArgs">RuleIdpDiscoveryArgs</a></span><span class="p">, </span><span class="nx">opts</span> ...<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#ResourceOption">pulumi.ResourceOption</a></span><span class="p">) (*<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi-okta/sdk/go/okta/policy?tab=doc#RuleIdpDiscovery">RuleIdpDiscovery</a></span>, error)</span></code></pre></div>
{{% /choosable %}}

{{% choosable language csharp %}}
<div class="highlight"><pre class="chroma"><code class="language-csharp" data-lang="csharp"><span class="k">public </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi.Okta/Pulumi.Okta.Policy.RuleIdpDiscovery.html">RuleIdpDiscovery</a></span><span class="p">(</span><span class="nx"><a href="https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/built-in-types">string</a></span> <span class="nx">name<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi.Okta/Pulumi.Okta.Policy.RuleIdpDiscoveryArgs.html">RuleIdpDiscoveryArgs</a></span> <span class="nx">args<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi/Pulumi.CustomResourceOptions.html">CustomResourceOptions</a></span>? <span class="nx">opts = null<span class="p">)</span></code></pre></div>
{{% /choosable %}}

{{% choosable language nodejs %}}

<dl class="resources-properties">
    <dt class="property-required" title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The unique name of the resource.</dd>
    <dt class="property-optional" title="Optional">
        <span>args</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The arguments to use to populate this resource's properties.</dd>
    <dt class="property-optional" title="Optional">
        <span>opts</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>A bag of options that control this resource's behavior.</dd>
</dl>

{{% /choosable %}}

{{% choosable language python %}}
<dl class="resources-properties">
    <dt class="property-required" title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The unique name of the resource.</dd>
    <dt class="property-optional" title="Optional">
        <span>opts</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>A bag of options that control this resource's behavior.</dd>
</dl>
{{% /choosable %}}

{{% choosable language go %}}

<dl class="resources-properties">
    <dt class="property-required" title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The unique name of the resource.</dd>
    <dt class="property-optional" title="Optional">
        <span>args</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The arguments to use to populate this resource's properties.</dd>
    <dt class="property-optional" title="Optional">
        <span>opts</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>A bag of options that control this resource's behavior.</dd>
</dl>

{{% /choosable %}}

{{% choosable language csharp %}}

<dl class="resources-properties">
    <dt class="property-required" title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The unique name of the resource.</dd>
    <dt class="property-optional" title="Optional">
        <span>args</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The arguments to use to populate this resource's properties.</dd>
    <dt class="property-optional" title="Optional">
        <span>opts</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>A bag of options that control this resource's behavior.</dd>
</dl>

{{% /choosable %}}

#### Resource Arguments




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>App<wbr>Excludes</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#ruleidpdiscoveryappexclude">List&lt;Rule<wbr>Idp<wbr>Discovery<wbr>App<wbr>Exclude<wbr>Args&gt;?</a></span>
    </dt>
    <dd>{{% md %}}Applications to exclude in discovery rule
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>App<wbr>Includes</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#ruleidpdiscoveryappinclude">List&lt;Rule<wbr>Idp<wbr>Discovery<wbr>App<wbr>Include<wbr>Args&gt;?</a></span>
    </dt>
    <dd>{{% md %}}Applications to include in discovery rule
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Idp<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Idp<wbr>Type</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Policy Rule Name.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Network<wbr>Connection</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Network selection mode: `"ANYWHERE"`, `"ZONE"`, `"ON_NETWORK"`, or `"OFF_NETWORK"`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Network<wbr>Excludes</span>
        <span class="property-indicator"></span>
        <span class="property-type">List<string>?</span>
    </dt>
    <dd>{{% md %}}The network zones to exclude. Conflicts with `network_includes`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Network<wbr>Includes</span>
        <span class="property-indicator"></span>
        <span class="property-type">List<string>?</span>
    </dt>
    <dd>{{% md %}}The network zones to include. Conflicts with `network_excludes`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Platform<wbr>Includes</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#ruleidpdiscoveryplatforminclude">List&lt;Rule<wbr>Idp<wbr>Discovery<wbr>Platform<wbr>Include<wbr>Args&gt;?</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Policyid</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Policy ID.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Priority</span>
        <span class="property-indicator"></span>
        <span class="property-type">int?</span>
    </dt>
    <dd>{{% md %}}Policy Rule Priority, this attribute can be set to a valid priority. To avoid endless diff situation we error if an invalid priority is provided. API defaults it to the last/lowest if not there.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Status</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Policy Rule Status: `"ACTIVE"` or `"INACTIVE"`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>User<wbr>Identifier<wbr>Attribute</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>User<wbr>Identifier<wbr>Patterns</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#ruleidpdiscoveryuseridentifierpattern">List&lt;Rule<wbr>Idp<wbr>Discovery<wbr>User<wbr>Identifier<wbr>Pattern<wbr>Args&gt;?</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>User<wbr>Identifier<wbr>Type</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>App<wbr>Excludes</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#ruleidpdiscoveryappexclude">[]Rule<wbr>Idp<wbr>Discovery<wbr>App<wbr>Exclude</a></span>
    </dt>
    <dd>{{% md %}}Applications to exclude in discovery rule
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>App<wbr>Includes</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#ruleidpdiscoveryappinclude">[]Rule<wbr>Idp<wbr>Discovery<wbr>App<wbr>Include</a></span>
    </dt>
    <dd>{{% md %}}Applications to include in discovery rule
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Idp<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Idp<wbr>Type</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}Policy Rule Name.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Network<wbr>Connection</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}Network selection mode: `"ANYWHERE"`, `"ZONE"`, `"ON_NETWORK"`, or `"OFF_NETWORK"`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Network<wbr>Excludes</span>
        <span class="property-indicator"></span>
        <span class="property-type">[]string</span>
    </dt>
    <dd>{{% md %}}The network zones to exclude. Conflicts with `network_includes`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Network<wbr>Includes</span>
        <span class="property-indicator"></span>
        <span class="property-type">[]string</span>
    </dt>
    <dd>{{% md %}}The network zones to include. Conflicts with `network_excludes`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Platform<wbr>Includes</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#ruleidpdiscoveryplatforminclude">[]Rule<wbr>Idp<wbr>Discovery<wbr>Platform<wbr>Include</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Policyid</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Policy ID.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Priority</span>
        <span class="property-indicator"></span>
        <span class="property-type">*int</span>
    </dt>
    <dd>{{% md %}}Policy Rule Priority, this attribute can be set to a valid priority. To avoid endless diff situation we error if an invalid priority is provided. API defaults it to the last/lowest if not there.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Status</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}Policy Rule Status: `"ACTIVE"` or `"INACTIVE"`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>User<wbr>Identifier<wbr>Attribute</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>User<wbr>Identifier<wbr>Patterns</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#ruleidpdiscoveryuseridentifierpattern">[]Rule<wbr>Idp<wbr>Discovery<wbr>User<wbr>Identifier<wbr>Pattern</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>User<wbr>Identifier<wbr>Type</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>app<wbr>Excludes</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#ruleidpdiscoveryappexclude">Rule<wbr>Idp<wbr>Discovery<wbr>App<wbr>Exclude[]?</a></span>
    </dt>
    <dd>{{% md %}}Applications to exclude in discovery rule
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>app<wbr>Includes</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#ruleidpdiscoveryappinclude">Rule<wbr>Idp<wbr>Discovery<wbr>App<wbr>Include[]?</a></span>
    </dt>
    <dd>{{% md %}}Applications to include in discovery rule
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>idp<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>idp<wbr>Type</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Policy Rule Name.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>network<wbr>Connection</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Network selection mode: `"ANYWHERE"`, `"ZONE"`, `"ON_NETWORK"`, or `"OFF_NETWORK"`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>network<wbr>Excludes</span>
        <span class="property-indicator"></span>
        <span class="property-type">string[]?</span>
    </dt>
    <dd>{{% md %}}The network zones to exclude. Conflicts with `network_includes`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>network<wbr>Includes</span>
        <span class="property-indicator"></span>
        <span class="property-type">string[]?</span>
    </dt>
    <dd>{{% md %}}The network zones to include. Conflicts with `network_excludes`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>platform<wbr>Includes</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#ruleidpdiscoveryplatforminclude">Rule<wbr>Idp<wbr>Discovery<wbr>Platform<wbr>Include[]?</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>policyid</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Policy ID.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>priority</span>
        <span class="property-indicator"></span>
        <span class="property-type">number?</span>
    </dt>
    <dd>{{% md %}}Policy Rule Priority, this attribute can be set to a valid priority. To avoid endless diff situation we error if an invalid priority is provided. API defaults it to the last/lowest if not there.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>status</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Policy Rule Status: `"ACTIVE"` or `"INACTIVE"`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>user<wbr>Identifier<wbr>Attribute</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>user<wbr>Identifier<wbr>Patterns</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#ruleidpdiscoveryuseridentifierpattern">Rule<wbr>Idp<wbr>Discovery<wbr>User<wbr>Identifier<wbr>Pattern[]?</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>user<wbr>Identifier<wbr>Type</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>app_<wbr>excludes</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#ruleidpdiscoveryappexclude">List[Rule<wbr>Idp<wbr>Discovery<wbr>App<wbr>Exclude]</a></span>
    </dt>
    <dd>{{% md %}}Applications to exclude in discovery rule
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>app_<wbr>includes</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#ruleidpdiscoveryappinclude">List[Rule<wbr>Idp<wbr>Discovery<wbr>App<wbr>Include]</a></span>
    </dt>
    <dd>{{% md %}}Applications to include in discovery rule
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>idp_<wbr>id</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>idp_<wbr>type</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Policy Rule Name.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>network_<wbr>connection</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Network selection mode: `"ANYWHERE"`, `"ZONE"`, `"ON_NETWORK"`, or `"OFF_NETWORK"`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>network_<wbr>excludes</span>
        <span class="property-indicator"></span>
        <span class="property-type">List[str]</span>
    </dt>
    <dd>{{% md %}}The network zones to exclude. Conflicts with `network_includes`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>network_<wbr>includes</span>
        <span class="property-indicator"></span>
        <span class="property-type">List[str]</span>
    </dt>
    <dd>{{% md %}}The network zones to include. Conflicts with `network_excludes`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>platform_<wbr>includes</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#ruleidpdiscoveryplatforminclude">List[Rule<wbr>Idp<wbr>Discovery<wbr>Platform<wbr>Include]</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>policyid</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Policy ID.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>priority</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}Policy Rule Priority, this attribute can be set to a valid priority. To avoid endless diff situation we error if an invalid priority is provided. API defaults it to the last/lowest if not there.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>status</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Policy Rule Status: `"ACTIVE"` or `"INACTIVE"`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>user_<wbr>identifier_<wbr>attribute</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>user_<wbr>identifier_<wbr>patterns</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#ruleidpdiscoveryuseridentifierpattern">List[Rule<wbr>Idp<wbr>Discovery<wbr>User<wbr>Identifier<wbr>Pattern]</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>user_<wbr>identifier_<wbr>type</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

</dl>
{{% /choosable %}}







## RuleIdpDiscovery Output Properties

The following output properties are available:




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-"
            title="">
        <span>App<wbr>Excludes</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#ruleidpdiscoveryappexclude">List&lt;Rule<wbr>Idp<wbr>Discovery<wbr>App<wbr>Exclude&gt;?</a></span>
    </dt>
    <dd>{{% md %}}Applications to exclude in discovery rule
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>App<wbr>Includes</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#ruleidpdiscoveryappinclude">List&lt;Rule<wbr>Idp<wbr>Discovery<wbr>App<wbr>Include&gt;?</a></span>
    </dt>
    <dd>{{% md %}}Applications to include in discovery rule
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Idp<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Idp<wbr>Type</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Policy Rule Name.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Network<wbr>Connection</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Network selection mode: `"ANYWHERE"`, `"ZONE"`, `"ON_NETWORK"`, or `"OFF_NETWORK"`.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Network<wbr>Excludes</span>
        <span class="property-indicator"></span>
        <span class="property-type">List<string>?</span>
    </dt>
    <dd>{{% md %}}The network zones to exclude. Conflicts with `network_includes`.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Network<wbr>Includes</span>
        <span class="property-indicator"></span>
        <span class="property-type">List<string>?</span>
    </dt>
    <dd>{{% md %}}The network zones to include. Conflicts with `network_excludes`.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Platform<wbr>Includes</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#ruleidpdiscoveryplatforminclude">List&lt;Rule<wbr>Idp<wbr>Discovery<wbr>Platform<wbr>Include&gt;?</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Policyid</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Policy ID.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Priority</span>
        <span class="property-indicator"></span>
        <span class="property-type">int?</span>
    </dt>
    <dd>{{% md %}}Policy Rule Priority, this attribute can be set to a valid priority. To avoid endless diff situation we error if an invalid priority is provided. API defaults it to the last/lowest if not there.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Status</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Policy Rule Status: `"ACTIVE"` or `"INACTIVE"`.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>User<wbr>Identifier<wbr>Attribute</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>User<wbr>Identifier<wbr>Patterns</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#ruleidpdiscoveryuseridentifierpattern">List&lt;Rule<wbr>Idp<wbr>Discovery<wbr>User<wbr>Identifier<wbr>Pattern&gt;?</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>User<wbr>Identifier<wbr>Type</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-"
            title="">
        <span>App<wbr>Excludes</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#ruleidpdiscoveryappexclude">[]Rule<wbr>Idp<wbr>Discovery<wbr>App<wbr>Exclude</a></span>
    </dt>
    <dd>{{% md %}}Applications to exclude in discovery rule
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>App<wbr>Includes</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#ruleidpdiscoveryappinclude">[]Rule<wbr>Idp<wbr>Discovery<wbr>App<wbr>Include</a></span>
    </dt>
    <dd>{{% md %}}Applications to include in discovery rule
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Idp<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Idp<wbr>Type</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Policy Rule Name.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Network<wbr>Connection</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}Network selection mode: `"ANYWHERE"`, `"ZONE"`, `"ON_NETWORK"`, or `"OFF_NETWORK"`.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Network<wbr>Excludes</span>
        <span class="property-indicator"></span>
        <span class="property-type">[]string</span>
    </dt>
    <dd>{{% md %}}The network zones to exclude. Conflicts with `network_includes`.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Network<wbr>Includes</span>
        <span class="property-indicator"></span>
        <span class="property-type">[]string</span>
    </dt>
    <dd>{{% md %}}The network zones to include. Conflicts with `network_excludes`.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Platform<wbr>Includes</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#ruleidpdiscoveryplatforminclude">[]Rule<wbr>Idp<wbr>Discovery<wbr>Platform<wbr>Include</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Policyid</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Policy ID.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Priority</span>
        <span class="property-indicator"></span>
        <span class="property-type">*int</span>
    </dt>
    <dd>{{% md %}}Policy Rule Priority, this attribute can be set to a valid priority. To avoid endless diff situation we error if an invalid priority is provided. API defaults it to the last/lowest if not there.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Status</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}Policy Rule Status: `"ACTIVE"` or `"INACTIVE"`.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>User<wbr>Identifier<wbr>Attribute</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>User<wbr>Identifier<wbr>Patterns</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#ruleidpdiscoveryuseridentifierpattern">[]Rule<wbr>Idp<wbr>Discovery<wbr>User<wbr>Identifier<wbr>Pattern</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>User<wbr>Identifier<wbr>Type</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-"
            title="">
        <span>app<wbr>Excludes</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#ruleidpdiscoveryappexclude">Rule<wbr>Idp<wbr>Discovery<wbr>App<wbr>Exclude[]?</a></span>
    </dt>
    <dd>{{% md %}}Applications to exclude in discovery rule
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>app<wbr>Includes</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#ruleidpdiscoveryappinclude">Rule<wbr>Idp<wbr>Discovery<wbr>App<wbr>Include[]?</a></span>
    </dt>
    <dd>{{% md %}}Applications to include in discovery rule
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>idp<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>idp<wbr>Type</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Policy Rule Name.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>network<wbr>Connection</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Network selection mode: `"ANYWHERE"`, `"ZONE"`, `"ON_NETWORK"`, or `"OFF_NETWORK"`.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>network<wbr>Excludes</span>
        <span class="property-indicator"></span>
        <span class="property-type">string[]?</span>
    </dt>
    <dd>{{% md %}}The network zones to exclude. Conflicts with `network_includes`.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>network<wbr>Includes</span>
        <span class="property-indicator"></span>
        <span class="property-type">string[]?</span>
    </dt>
    <dd>{{% md %}}The network zones to include. Conflicts with `network_excludes`.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>platform<wbr>Includes</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#ruleidpdiscoveryplatforminclude">Rule<wbr>Idp<wbr>Discovery<wbr>Platform<wbr>Include[]?</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>policyid</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Policy ID.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>priority</span>
        <span class="property-indicator"></span>
        <span class="property-type">number?</span>
    </dt>
    <dd>{{% md %}}Policy Rule Priority, this attribute can be set to a valid priority. To avoid endless diff situation we error if an invalid priority is provided. API defaults it to the last/lowest if not there.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>status</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Policy Rule Status: `"ACTIVE"` or `"INACTIVE"`.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>user<wbr>Identifier<wbr>Attribute</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>user<wbr>Identifier<wbr>Patterns</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#ruleidpdiscoveryuseridentifierpattern">Rule<wbr>Idp<wbr>Discovery<wbr>User<wbr>Identifier<wbr>Pattern[]?</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>user<wbr>Identifier<wbr>Type</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-"
            title="">
        <span>app_<wbr>excludes</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#ruleidpdiscoveryappexclude">List[Rule<wbr>Idp<wbr>Discovery<wbr>App<wbr>Exclude]</a></span>
    </dt>
    <dd>{{% md %}}Applications to exclude in discovery rule
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>app_<wbr>includes</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#ruleidpdiscoveryappinclude">List[Rule<wbr>Idp<wbr>Discovery<wbr>App<wbr>Include]</a></span>
    </dt>
    <dd>{{% md %}}Applications to include in discovery rule
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>idp_<wbr>id</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>idp_<wbr>type</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Policy Rule Name.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>network_<wbr>connection</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Network selection mode: `"ANYWHERE"`, `"ZONE"`, `"ON_NETWORK"`, or `"OFF_NETWORK"`.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>network_<wbr>excludes</span>
        <span class="property-indicator"></span>
        <span class="property-type">List[str]</span>
    </dt>
    <dd>{{% md %}}The network zones to exclude. Conflicts with `network_includes`.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>network_<wbr>includes</span>
        <span class="property-indicator"></span>
        <span class="property-type">List[str]</span>
    </dt>
    <dd>{{% md %}}The network zones to include. Conflicts with `network_excludes`.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>platform_<wbr>includes</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#ruleidpdiscoveryplatforminclude">List[Rule<wbr>Idp<wbr>Discovery<wbr>Platform<wbr>Include]</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>policyid</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Policy ID.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>priority</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}Policy Rule Priority, this attribute can be set to a valid priority. To avoid endless diff situation we error if an invalid priority is provided. API defaults it to the last/lowest if not there.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>status</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Policy Rule Status: `"ACTIVE"` or `"INACTIVE"`.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>user_<wbr>identifier_<wbr>attribute</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>user_<wbr>identifier_<wbr>patterns</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#ruleidpdiscoveryuseridentifierpattern">List[Rule<wbr>Idp<wbr>Discovery<wbr>User<wbr>Identifier<wbr>Pattern]</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>user_<wbr>identifier_<wbr>type</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

</dl>
{{% /choosable %}}








## Look up an Existing RuleIdpDiscovery Resource

Get an existing RuleIdpDiscovery resource's state with the given name, ID, and optional extra properties used to qualify the lookup.

{{< chooser language "javascript,typescript,python,go,csharp  " / >}}

{{% choosable language nodejs %}}
<div class="highlight"><pre class="chroma"><code class="language-typescript" data-lang="typescript"><span class="k">public static </span><span class="nf">get</span><span class="p">(</span><span class="nx">name</span>: <span class="nx"><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string">string</a></span><span class="p">, </span><span class="nx">id</span>: <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/pulumi/#ID">Input&lt;ID&gt;</a></span><span class="p">, </span><span class="nx">state</span>?: <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/okta/policy/#RuleIdpDiscoveryState">RuleIdpDiscoveryState</a></span><span class="p">, </span><span class="nx">opts</span>?: <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/pulumi/#CustomResourceOptions">CustomResourceOptions</a></span><span class="p">): </span><span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/okta/policy/#RuleIdpDiscovery">RuleIdpDiscovery</a></span></code></pre></div>
{{% /choosable %}}

{{% choosable language python %}}
<div class="highlight"><pre class="chroma"><code class="language-python" data-lang="python"><span class="k">static </span><span class="nf">get</span><span class="p">(resource_name, id, opts=None, </span>app_excludes=None<span class="p">, </span>app_includes=None<span class="p">, </span>idp_id=None<span class="p">, </span>idp_type=None<span class="p">, </span>name=None<span class="p">, </span>network_connection=None<span class="p">, </span>network_excludes=None<span class="p">, </span>network_includes=None<span class="p">, </span>platform_includes=None<span class="p">, </span>policyid=None<span class="p">, </span>priority=None<span class="p">, </span>status=None<span class="p">, </span>user_identifier_attribute=None<span class="p">, </span>user_identifier_patterns=None<span class="p">, </span>user_identifier_type=None<span class="p">, __props__=None);</span></code></pre></div>
{{% /choosable %}}

{{% choosable language go %}}
<div class="highlight"><pre class="chroma"><code class="language-go" data-lang="go"><span class="k">func </span>GetRuleIdpDiscovery<span class="p">(</span><span class="nx">ctx</span> *<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#Context">Context</a></span><span class="p">, </span><span class="nx">name</span> <span class="nx"><a href="https://golang.org/pkg/builtin/#string">string</a></span><span class="p">, </span><span class="nx">id</span> <span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#IDInput">IDInput</a></span><span class="p">, </span><span class="nx">state</span> *<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi-okta/sdk/go/okta/policy?tab=doc#RuleIdpDiscoveryState">RuleIdpDiscoveryState</a></span><span class="p">, </span><span class="nx">opts</span> ...<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#ResourceOption">ResourceOption</a></span><span class="p">) (*<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi-okta/sdk/go/okta/policy?tab=doc#RuleIdpDiscovery">RuleIdpDiscovery</a></span>, error)</span></code></pre></div>
{{% /choosable %}}

{{% choosable language csharp %}}
<div class="highlight"><pre class="chroma"><code class="language-csharp" data-lang="csharp"><span class="k">public static </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi.Okta/Pulumi.Okta.Policy.RuleIdpDiscovery.html">RuleIdpDiscovery</a></span><span class="nf"> Get</span><span class="p">(</span><span class="nx"><a href="https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/built-in-types">string</a></span> <span class="nx">name<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi/Pulumi.Input.html">Input&lt;string&gt;</a></span> <span class="nx">id<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi.Okta/Pulumi.Okta.Policy.RuleIdpDiscoveryState.html">RuleIdpDiscoveryState</a></span>? <span class="nx">state<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi/Pulumi.CustomResourceOptions.html">CustomResourceOptions</a></span>? <span class="nx">opts = null<span class="p">)</span></code></pre></div>
{{% /choosable %}}

{{% choosable language nodejs %}}

<dl class="resources-properties">
    <dt class="property-required" title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The unique name of the resulting resource.</dd>
    <dt class="property-required" title="Required">
        <span>id</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The <em>unique</em> provider ID of the resource to lookup.</dd>
    <dt class="property-optional" title="Optional">
        <span>state</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>Any extra arguments used during the lookup.</dd>
    <dt class="property-optional" title="Optional">
        <span>opts</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>A bag of options that control this resource's behavior.</dd>
</dl>

{{% /choosable %}}

{{% choosable language python %}}
<dl class="resources-properties">
    <dt class="property-required" title="Required">
        <span>resource_name</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The unique name of the resulting resource.</dd>
    <dt class="property-required" title="Optional">
        <span>id</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The <em>unique</em> provider ID of the resource to lookup.</dd>
</dl>
{{% /choosable %}}

{{% choosable language go %}}

<dl class="resources-properties">
    <dt class="property-required" title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The unique name of the resulting resource.</dd>
    <dt class="property-required" title="Required">
        <span>id</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The <em>unique</em> provider ID of the resource to lookup.</dd>
    <dt class="property-optional" title="Optional">
        <span>state</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>Any extra arguments used during the lookup.</dd>
    <dt class="property-optional" title="Optional">
        <span>opts</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>A bag of options that control this resource's behavior.</dd>
</dl>

{{% /choosable %}}

{{% choosable language csharp %}}

<dl class="resources-properties">
    <dt class="property-required" title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The unique name of the resulting resource.</dd>
    <dt class="property-required" title="Required">
        <span>id</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>The <em>unique</em> provider ID of the resource to lookup.</dd>
    <dt class="property-optional" title="Optional">
        <span>state</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>Any extra arguments used during the lookup.</dd>
    <dt class="property-optional" title="Optional">
        <span>opts</span>
        <span class="property-indicator"></span>
    </dt>
    <dd>A bag of options that control this resource's behavior.</dd>
</dl>

{{% /choosable %}}

The following state arguments are supported:



{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>App<wbr>Excludes</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#ruleidpdiscoveryappexclude">List&lt;Rule<wbr>Idp<wbr>Discovery<wbr>App<wbr>Exclude<wbr>Args&gt;?</a></span>
    </dt>
    <dd>{{% md %}}Applications to exclude in discovery rule
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>App<wbr>Includes</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#ruleidpdiscoveryappinclude">List&lt;Rule<wbr>Idp<wbr>Discovery<wbr>App<wbr>Include<wbr>Args&gt;?</a></span>
    </dt>
    <dd>{{% md %}}Applications to include in discovery rule
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Idp<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Idp<wbr>Type</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Policy Rule Name.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Network<wbr>Connection</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Network selection mode: `"ANYWHERE"`, `"ZONE"`, `"ON_NETWORK"`, or `"OFF_NETWORK"`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Network<wbr>Excludes</span>
        <span class="property-indicator"></span>
        <span class="property-type">List<string>?</span>
    </dt>
    <dd>{{% md %}}The network zones to exclude. Conflicts with `network_includes`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Network<wbr>Includes</span>
        <span class="property-indicator"></span>
        <span class="property-type">List<string>?</span>
    </dt>
    <dd>{{% md %}}The network zones to include. Conflicts with `network_excludes`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Platform<wbr>Includes</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#ruleidpdiscoveryplatforminclude">List&lt;Rule<wbr>Idp<wbr>Discovery<wbr>Platform<wbr>Include<wbr>Args&gt;?</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Policyid</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Policy ID.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Priority</span>
        <span class="property-indicator"></span>
        <span class="property-type">int?</span>
    </dt>
    <dd>{{% md %}}Policy Rule Priority, this attribute can be set to a valid priority. To avoid endless diff situation we error if an invalid priority is provided. API defaults it to the last/lowest if not there.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Status</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Policy Rule Status: `"ACTIVE"` or `"INACTIVE"`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>User<wbr>Identifier<wbr>Attribute</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>User<wbr>Identifier<wbr>Patterns</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#ruleidpdiscoveryuseridentifierpattern">List&lt;Rule<wbr>Idp<wbr>Discovery<wbr>User<wbr>Identifier<wbr>Pattern<wbr>Args&gt;?</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>User<wbr>Identifier<wbr>Type</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>App<wbr>Excludes</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#ruleidpdiscoveryappexclude">[]Rule<wbr>Idp<wbr>Discovery<wbr>App<wbr>Exclude</a></span>
    </dt>
    <dd>{{% md %}}Applications to exclude in discovery rule
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>App<wbr>Includes</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#ruleidpdiscoveryappinclude">[]Rule<wbr>Idp<wbr>Discovery<wbr>App<wbr>Include</a></span>
    </dt>
    <dd>{{% md %}}Applications to include in discovery rule
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Idp<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Idp<wbr>Type</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}Policy Rule Name.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Network<wbr>Connection</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}Network selection mode: `"ANYWHERE"`, `"ZONE"`, `"ON_NETWORK"`, or `"OFF_NETWORK"`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Network<wbr>Excludes</span>
        <span class="property-indicator"></span>
        <span class="property-type">[]string</span>
    </dt>
    <dd>{{% md %}}The network zones to exclude. Conflicts with `network_includes`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Network<wbr>Includes</span>
        <span class="property-indicator"></span>
        <span class="property-type">[]string</span>
    </dt>
    <dd>{{% md %}}The network zones to include. Conflicts with `network_excludes`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Platform<wbr>Includes</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#ruleidpdiscoveryplatforminclude">[]Rule<wbr>Idp<wbr>Discovery<wbr>Platform<wbr>Include</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Policyid</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}Policy ID.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Priority</span>
        <span class="property-indicator"></span>
        <span class="property-type">*int</span>
    </dt>
    <dd>{{% md %}}Policy Rule Priority, this attribute can be set to a valid priority. To avoid endless diff situation we error if an invalid priority is provided. API defaults it to the last/lowest if not there.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Status</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}Policy Rule Status: `"ACTIVE"` or `"INACTIVE"`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>User<wbr>Identifier<wbr>Attribute</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>User<wbr>Identifier<wbr>Patterns</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#ruleidpdiscoveryuseridentifierpattern">[]Rule<wbr>Idp<wbr>Discovery<wbr>User<wbr>Identifier<wbr>Pattern</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>User<wbr>Identifier<wbr>Type</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>app<wbr>Excludes</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#ruleidpdiscoveryappexclude">Rule<wbr>Idp<wbr>Discovery<wbr>App<wbr>Exclude[]?</a></span>
    </dt>
    <dd>{{% md %}}Applications to exclude in discovery rule
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>app<wbr>Includes</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#ruleidpdiscoveryappinclude">Rule<wbr>Idp<wbr>Discovery<wbr>App<wbr>Include[]?</a></span>
    </dt>
    <dd>{{% md %}}Applications to include in discovery rule
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>idp<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>idp<wbr>Type</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Policy Rule Name.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>network<wbr>Connection</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Network selection mode: `"ANYWHERE"`, `"ZONE"`, `"ON_NETWORK"`, or `"OFF_NETWORK"`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>network<wbr>Excludes</span>
        <span class="property-indicator"></span>
        <span class="property-type">string[]?</span>
    </dt>
    <dd>{{% md %}}The network zones to exclude. Conflicts with `network_includes`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>network<wbr>Includes</span>
        <span class="property-indicator"></span>
        <span class="property-type">string[]?</span>
    </dt>
    <dd>{{% md %}}The network zones to include. Conflicts with `network_excludes`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>platform<wbr>Includes</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#ruleidpdiscoveryplatforminclude">Rule<wbr>Idp<wbr>Discovery<wbr>Platform<wbr>Include[]?</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>policyid</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Policy ID.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>priority</span>
        <span class="property-indicator"></span>
        <span class="property-type">number?</span>
    </dt>
    <dd>{{% md %}}Policy Rule Priority, this attribute can be set to a valid priority. To avoid endless diff situation we error if an invalid priority is provided. API defaults it to the last/lowest if not there.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>status</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Policy Rule Status: `"ACTIVE"` or `"INACTIVE"`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>user<wbr>Identifier<wbr>Attribute</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>user<wbr>Identifier<wbr>Patterns</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#ruleidpdiscoveryuseridentifierpattern">Rule<wbr>Idp<wbr>Discovery<wbr>User<wbr>Identifier<wbr>Pattern[]?</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>user<wbr>Identifier<wbr>Type</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>app_<wbr>excludes</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#ruleidpdiscoveryappexclude">List[Rule<wbr>Idp<wbr>Discovery<wbr>App<wbr>Exclude]</a></span>
    </dt>
    <dd>{{% md %}}Applications to exclude in discovery rule
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>app_<wbr>includes</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#ruleidpdiscoveryappinclude">List[Rule<wbr>Idp<wbr>Discovery<wbr>App<wbr>Include]</a></span>
    </dt>
    <dd>{{% md %}}Applications to include in discovery rule
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>idp_<wbr>id</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>idp_<wbr>type</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Policy Rule Name.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>network_<wbr>connection</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Network selection mode: `"ANYWHERE"`, `"ZONE"`, `"ON_NETWORK"`, or `"OFF_NETWORK"`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>network_<wbr>excludes</span>
        <span class="property-indicator"></span>
        <span class="property-type">List[str]</span>
    </dt>
    <dd>{{% md %}}The network zones to exclude. Conflicts with `network_includes`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>network_<wbr>includes</span>
        <span class="property-indicator"></span>
        <span class="property-type">List[str]</span>
    </dt>
    <dd>{{% md %}}The network zones to include. Conflicts with `network_excludes`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>platform_<wbr>includes</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#ruleidpdiscoveryplatforminclude">List[Rule<wbr>Idp<wbr>Discovery<wbr>Platform<wbr>Include]</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>policyid</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Policy ID.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>priority</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}Policy Rule Priority, this attribute can be set to a valid priority. To avoid endless diff situation we error if an invalid priority is provided. API defaults it to the last/lowest if not there.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>status</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Policy Rule Status: `"ACTIVE"` or `"INACTIVE"`.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>user_<wbr>identifier_<wbr>attribute</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>user_<wbr>identifier_<wbr>patterns</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#ruleidpdiscoveryuseridentifierpattern">List[Rule<wbr>Idp<wbr>Discovery<wbr>User<wbr>Identifier<wbr>Pattern]</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>user_<wbr>identifier_<wbr>type</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

</dl>
{{% /choosable %}}










## Supporting Types

<h4>Rule<wbr>Idp<wbr>Discovery<wbr>App<wbr>Exclude</h4>
{{% choosable language nodejs %}}
> See the <a href="/docs/reference/pkg/nodejs/pulumi/okta/types/input/#RuleIdpDiscoveryAppExclude">input</a> and <a href="/docs/reference/pkg/nodejs/pulumi/okta/types/output/#RuleIdpDiscoveryAppExclude">output</a> API doc for this type.
{{% /choosable %}}

{{% choosable language go %}}
> See the <a href="https://pkg.go.dev/github.com/pulumi/pulumi-okta/sdk/go/okta/policy?tab=doc#RuleIdpDiscoveryAppExcludeArgs">input</a> and <a href="https://pkg.go.dev/github.com/pulumi/pulumi-okta/sdk/go/okta/policy?tab=doc#RuleIdpDiscoveryAppExcludeOutput">output</a> API doc for this type.
{{% /choosable %}}




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}ID of the Rule.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Policy Rule Name.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Type</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}ID of the Rule.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}Policy Rule Name.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Type</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}ID of the Rule.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Policy Rule Name.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>type</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>id</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}ID of the Rule.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Policy Rule Name.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>type</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

</dl>
{{% /choosable %}}





<h4>Rule<wbr>Idp<wbr>Discovery<wbr>App<wbr>Include</h4>
{{% choosable language nodejs %}}
> See the <a href="/docs/reference/pkg/nodejs/pulumi/okta/types/input/#RuleIdpDiscoveryAppInclude">input</a> and <a href="/docs/reference/pkg/nodejs/pulumi/okta/types/output/#RuleIdpDiscoveryAppInclude">output</a> API doc for this type.
{{% /choosable %}}

{{% choosable language go %}}
> See the <a href="https://pkg.go.dev/github.com/pulumi/pulumi-okta/sdk/go/okta/policy?tab=doc#RuleIdpDiscoveryAppIncludeArgs">input</a> and <a href="https://pkg.go.dev/github.com/pulumi/pulumi-okta/sdk/go/okta/policy?tab=doc#RuleIdpDiscoveryAppIncludeOutput">output</a> API doc for this type.
{{% /choosable %}}




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}ID of the Rule.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Policy Rule Name.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Type</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}ID of the Rule.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}Policy Rule Name.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Type</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}ID of the Rule.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Policy Rule Name.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>type</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>id</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}ID of the Rule.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Policy Rule Name.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>type</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

</dl>
{{% /choosable %}}





<h4>Rule<wbr>Idp<wbr>Discovery<wbr>Platform<wbr>Include</h4>
{{% choosable language nodejs %}}
> See the <a href="/docs/reference/pkg/nodejs/pulumi/okta/types/input/#RuleIdpDiscoveryPlatformInclude">input</a> and <a href="/docs/reference/pkg/nodejs/pulumi/okta/types/output/#RuleIdpDiscoveryPlatformInclude">output</a> API doc for this type.
{{% /choosable %}}

{{% choosable language go %}}
> See the <a href="https://pkg.go.dev/github.com/pulumi/pulumi-okta/sdk/go/okta/policy?tab=doc#RuleIdpDiscoveryPlatformIncludeArgs">input</a> and <a href="https://pkg.go.dev/github.com/pulumi/pulumi-okta/sdk/go/okta/policy?tab=doc#RuleIdpDiscoveryPlatformIncludeOutput">output</a> API doc for this type.
{{% /choosable %}}




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Os<wbr>Expression</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Os<wbr>Type</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Type</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Os<wbr>Expression</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Os<wbr>Type</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Type</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>os<wbr>Expression</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>os<wbr>Type</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>type</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>os<wbr>Expression</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>os<wbr>Type</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>type</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

</dl>
{{% /choosable %}}





<h4>Rule<wbr>Idp<wbr>Discovery<wbr>User<wbr>Identifier<wbr>Pattern</h4>
{{% choosable language nodejs %}}
> See the <a href="/docs/reference/pkg/nodejs/pulumi/okta/types/input/#RuleIdpDiscoveryUserIdentifierPattern">input</a> and <a href="/docs/reference/pkg/nodejs/pulumi/okta/types/output/#RuleIdpDiscoveryUserIdentifierPattern">output</a> API doc for this type.
{{% /choosable %}}

{{% choosable language go %}}
> See the <a href="https://pkg.go.dev/github.com/pulumi/pulumi-okta/sdk/go/okta/policy?tab=doc#RuleIdpDiscoveryUserIdentifierPatternArgs">input</a> and <a href="https://pkg.go.dev/github.com/pulumi/pulumi-okta/sdk/go/okta/policy?tab=doc#RuleIdpDiscoveryUserIdentifierPatternOutput">output</a> API doc for this type.
{{% /choosable %}}




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Match<wbr>Type</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Value</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Match<wbr>Type</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Value</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>match<wbr>Type</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>value</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>match_<wbr>type</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>value</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

</dl>
{{% /choosable %}}









<h3>Package Details</h3>
<dl class="package-details">
	<dt>Repository</dt>
	<dd><a href="https://github.com/pulumi/pulumi-okta">https://github.com/pulumi/pulumi-okta</a></dd>
	<dt>License</dt>
	<dd>Apache-2.0</dd>
    
</dl>
