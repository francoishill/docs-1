---
title: "Module jira"
title_tag: "Module jira | Package @pulumi/signalfx | Node.js SDK"
linktitle: "jira"
meta_desc: "Explore members of the jira module in the @pulumi/signalfx package."
git_sha: "259fb9aba5c29d4cf535ca6c12ce9c3129fd56ab"
block_external_search_index: true
---

<!-- WARNING: this page was generated by a tool. Do not edit it by hand. -->
<!-- To change it, please see https://github.com/pulumi/docs/tree/master/tools/tscdocgen. -->

{{< resource-docs-alert "signalfx" >}}




<h3>Resources</h3>
<ul class="api">
    <li><a href="#Integration"><span class="symbol resource"></span>Integration</a></li>
</ul>


<h3>Others</h3>
<ul class="api">
    <li><a href="#IntegrationArgs"><span class="symbol api"></span>IntegrationArgs</a></li>
    <li><a href="#IntegrationState"><span class="symbol api"></span>IntegrationState</a></li>
</ul>


<h2 id="resources">Resources</h2>
<h3 class="pdoc-module-header" id="Integration" data-link-title="Integration">
    <a href="https://github.com/pulumi/pulumi-signalfx/blob/259fb9aba5c29d4cf535ca6c12ce9c3129fd56ab/sdk/nodejs/jira/integration.ts#L33">
        Resource <strong>Integration</strong>
    </a>
</h3>

<pre class="highlight"><code><span class='kr'>class</span> <span class='nx'>Integration</span> <span class='kr'>extends</span> <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#CustomResource'>CustomResource</a></code></pre>

SignalFx Jira integrations. For help with this integration see [Integration with Jira](https://docs.signalfx.com/en/latest/admin-guide/integrate-notifications.html#integrate-with-jira).

> **NOTE** When managing integrations you'll need to use an admin token to authenticate the SignalFx provider. Otherwise you'll receive a 4xx error.

#### Example Usage



```typescript
import * as pulumi from "@pulumi/pulumi";
import * as signalfx from "@pulumi/signalfx";

const jiraMyteamXX = new signalfx.jira.Integration("jira_myteamXX", {
    assigneeDisplayName: "Testy Testerson",
    assigneeName: "testytesterson",
    authMethod: "UsernameAndPassword",
    baseUrl: "https://www.example.com",
    enabled: false,
    issueType: "Story",
    password: "paasword",
    projectKey: "TEST",
    username: "yoosername",
});
```

<h4 class="pdoc-member-header" id="Integration-constructor">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-signalfx/blob/259fb9aba5c29d4cf535ca6c12ce9c3129fd56ab/sdk/nodejs/jira/integration.ts#L108"> <b>constructor</b></a>
</h4>


<pre class="highlight"><code><span class='kd'></span><span class='kd'>new</span> Integration(name: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>, args: <a href='#IntegrationArgs'>IntegrationArgs</a>, opts?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#CustomResourceOptions'>pulumi.CustomResourceOptions</a>)</code></pre>


Create a Integration resource with the given unique name, arguments, and options.

* `name` The _unique_ name of the resource.
* `args` The arguments to use to populate this resource&#39;s properties.
* `opts` A bag of options that control this resource&#39;s behavior.

<h4 class="pdoc-member-header" id="Integration-get">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-signalfx/blob/259fb9aba5c29d4cf535ca6c12ce9c3129fd56ab/sdk/nodejs/jira/integration.ts#L43">method <b>get</b></a>
</h4>


<pre class="highlight"><code><span class='kd'>public static </span>get(name: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>, id: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#ID'>pulumi.ID</a>&gt;, state?: <a href='#IntegrationState'>IntegrationState</a>, opts?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#CustomResourceOptions'>pulumi.CustomResourceOptions</a>): <a href='#Integration'>Integration</a></code></pre>


Get an existing Integration resource's state with the given name, ID, and optional extra
properties used to qualify the lookup.

<h4 class="pdoc-member-header" id="Integration-getProvider">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-signalfx/blob/259fb9aba5c29d4cf535ca6c12ce9c3129fd56ab/sdk/nodejs/jira/integration.ts#L33">method <b>getProvider</b></a>
</h4>


<pre class="highlight"><code><span class='kd'></span>getProvider(moduleMember: <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>): <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#ProviderResource'>ProviderResource</a> | <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span></code></pre>

<h4 class="pdoc-member-header" id="Integration-isInstance">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-signalfx/blob/259fb9aba5c29d4cf535ca6c12ce9c3129fd56ab/sdk/nodejs/jira/integration.ts#L54">method <b>isInstance</b></a>
</h4>


<pre class="highlight"><code><span class='kd'>public static </span>isInstance(obj: <span class='kd'><a href='https://www.typescriptlang.org/docs/handbook/basic-types.html#any'>any</a></span>): obj is Integration</code></pre>


Returns true if the given object is an instance of Integration.  This is designed to work even
when multiple copies of the Pulumi SDK have been loaded into the same process.

<h4 class="pdoc-member-header" id="Integration-apiToken">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-signalfx/blob/259fb9aba5c29d4cf535ca6c12ce9c3129fd56ab/sdk/nodejs/jira/integration.ts#L64">property <b>apiToken</b></a>
</h4>

<pre class="highlight"><code><span class='kd'>public </span>apiToken: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span> | <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span>&gt;;</code></pre>

The API token for the user email

<h4 class="pdoc-member-header" id="Integration-assigneeDisplayName">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-signalfx/blob/259fb9aba5c29d4cf535ca6c12ce9c3129fd56ab/sdk/nodejs/jira/integration.ts#L68">property <b>assigneeDisplayName</b></a>
</h4>

<pre class="highlight"><code><span class='kd'>public </span>assigneeDisplayName: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span> | <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span>&gt;;</code></pre>

Jira display name for the assignee.

<h4 class="pdoc-member-header" id="Integration-assigneeName">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-signalfx/blob/259fb9aba5c29d4cf535ca6c12ce9c3129fd56ab/sdk/nodejs/jira/integration.ts#L72">property <b>assigneeName</b></a>
</h4>

<pre class="highlight"><code><span class='kd'>public </span>assigneeName: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</code></pre>

Jira user name for the assignee.

<h4 class="pdoc-member-header" id="Integration-authMethod">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-signalfx/blob/259fb9aba5c29d4cf535ca6c12ce9c3129fd56ab/sdk/nodejs/jira/integration.ts#L76">property <b>authMethod</b></a>
</h4>

<pre class="highlight"><code><span class='kd'>public </span>authMethod: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</code></pre>

Authentication method used when creating the Jira integration. One of `EmailAndToken` (using `userEmail` and `apiToken`) or `UsernameAndPassword` (using `username` and `password`).

<h4 class="pdoc-member-header" id="Integration-baseUrl">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-signalfx/blob/259fb9aba5c29d4cf535ca6c12ce9c3129fd56ab/sdk/nodejs/jira/integration.ts#L80">property <b>baseUrl</b></a>
</h4>

<pre class="highlight"><code><span class='kd'>public </span>baseUrl: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</code></pre>

Base URL of the Jira instance that's integrated with SignalFx.

<h4 class="pdoc-member-header" id="Integration-enabled">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-signalfx/blob/259fb9aba5c29d4cf535ca6c12ce9c3129fd56ab/sdk/nodejs/jira/integration.ts#L84">property <b>enabled</b></a>
</h4>

<pre class="highlight"><code><span class='kd'>public </span>enabled: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean'>boolean</a></span>&gt;;</code></pre>

Whether the integration is enabled.

<h4 class="pdoc-member-header" id="Integration-id">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-signalfx/blob/259fb9aba5c29d4cf535ca6c12ce9c3129fd56ab/sdk/nodejs/jira/integration.ts#L33">property <b>id</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>id: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>Output</a>&lt;<a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#ID'>ID</a>&gt;;</code></pre>

id is the provider-assigned unique ID for this managed resource.  It is set during
deployments and may be missing (undefined) during planning phases.

<h4 class="pdoc-member-header" id="Integration-issueType">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-signalfx/blob/259fb9aba5c29d4cf535ca6c12ce9c3129fd56ab/sdk/nodejs/jira/integration.ts#L88">property <b>issueType</b></a>
</h4>

<pre class="highlight"><code><span class='kd'>public </span>issueType: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</code></pre>

Issue type (for example, Story) for tickets that Jira creates for detector notifications. SignalFx validates issue types, so you must specify a type that's valid for the Jira project specified in `projectKey`.

<h4 class="pdoc-member-header" id="Integration-name">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-signalfx/blob/259fb9aba5c29d4cf535ca6c12ce9c3129fd56ab/sdk/nodejs/jira/integration.ts#L92">property <b>name</b></a>
</h4>

<pre class="highlight"><code><span class='kd'>public </span>name: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</code></pre>

Name of the integration.

<h4 class="pdoc-member-header" id="Integration-password">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-signalfx/blob/259fb9aba5c29d4cf535ca6c12ce9c3129fd56ab/sdk/nodejs/jira/integration.ts#L96">property <b>password</b></a>
</h4>

<pre class="highlight"><code><span class='kd'>public </span>password: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span> | <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span>&gt;;</code></pre>

Password used to authenticate the Jira integration.

<h4 class="pdoc-member-header" id="Integration-projectKey">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-signalfx/blob/259fb9aba5c29d4cf535ca6c12ce9c3129fd56ab/sdk/nodejs/jira/integration.ts#L100">property <b>projectKey</b></a>
</h4>

<pre class="highlight"><code><span class='kd'>public </span>projectKey: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</code></pre>

Jira key of an existing project. When Jira creates a new ticket for a detector notification, the ticket is assigned to this project.

<h4 class="pdoc-member-header" id="Integration-urn">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-signalfx/blob/259fb9aba5c29d4cf535ca6c12ce9c3129fd56ab/sdk/nodejs/jira/integration.ts#L33">property <b>urn</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>urn: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>Output</a>&lt;<a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#URN'>URN</a>&gt;;</code></pre>

urn is the stable logical URN used to distinctly address a resource, both before and after
deployments.

<h4 class="pdoc-member-header" id="Integration-userEmail">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-signalfx/blob/259fb9aba5c29d4cf535ca6c12ce9c3129fd56ab/sdk/nodejs/jira/integration.ts#L104">property <b>userEmail</b></a>
</h4>

<pre class="highlight"><code><span class='kd'>public </span>userEmail: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span> | <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span>&gt;;</code></pre>

Email address used to authenticate the Jira integration.

<h4 class="pdoc-member-header" id="Integration-username">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-signalfx/blob/259fb9aba5c29d4cf535ca6c12ce9c3129fd56ab/sdk/nodejs/jira/integration.ts#L108">property <b>username</b></a>
</h4>

<pre class="highlight"><code><span class='kd'>public </span>username: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Output'>pulumi.Output</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span> | <span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/undefined'>undefined</a></span>&gt;;</code></pre>

User name used to authenticate the Jira integration.



<h2 id="apis">Others</h2>
<h3 class="pdoc-module-header" id="IntegrationArgs" data-link-title="IntegrationArgs">
    <a href="https://github.com/pulumi/pulumi-signalfx/blob/259fb9aba5c29d4cf535ca6c12ce9c3129fd56ab/sdk/nodejs/jira/integration.ts#L235">
        interface <strong>IntegrationArgs</strong>
    </a>
</h3>

<pre class="highlight"><code><span class='kr'>interface</span> <span class='nx'>IntegrationArgs</span></code></pre>

The set of arguments for constructing a Integration resource.

<h4 class="pdoc-member-header" id="IntegrationArgs-apiToken">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-signalfx/blob/259fb9aba5c29d4cf535ca6c12ce9c3129fd56ab/sdk/nodejs/jira/integration.ts#L239">property <b>apiToken</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>apiToken?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</code></pre>

The API token for the user email

<h4 class="pdoc-member-header" id="IntegrationArgs-assigneeDisplayName">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-signalfx/blob/259fb9aba5c29d4cf535ca6c12ce9c3129fd56ab/sdk/nodejs/jira/integration.ts#L243">property <b>assigneeDisplayName</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>assigneeDisplayName?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</code></pre>

Jira display name for the assignee.

<h4 class="pdoc-member-header" id="IntegrationArgs-assigneeName">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-signalfx/blob/259fb9aba5c29d4cf535ca6c12ce9c3129fd56ab/sdk/nodejs/jira/integration.ts#L247">property <b>assigneeName</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>assigneeName: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</code></pre>

Jira user name for the assignee.

<h4 class="pdoc-member-header" id="IntegrationArgs-authMethod">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-signalfx/blob/259fb9aba5c29d4cf535ca6c12ce9c3129fd56ab/sdk/nodejs/jira/integration.ts#L251">property <b>authMethod</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>authMethod: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</code></pre>

Authentication method used when creating the Jira integration. One of `EmailAndToken` (using `userEmail` and `apiToken`) or `UsernameAndPassword` (using `username` and `password`).

<h4 class="pdoc-member-header" id="IntegrationArgs-baseUrl">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-signalfx/blob/259fb9aba5c29d4cf535ca6c12ce9c3129fd56ab/sdk/nodejs/jira/integration.ts#L255">property <b>baseUrl</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>baseUrl: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</code></pre>

Base URL of the Jira instance that's integrated with SignalFx.

<h4 class="pdoc-member-header" id="IntegrationArgs-enabled">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-signalfx/blob/259fb9aba5c29d4cf535ca6c12ce9c3129fd56ab/sdk/nodejs/jira/integration.ts#L259">property <b>enabled</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>enabled: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean'>boolean</a></span>&gt;;</code></pre>

Whether the integration is enabled.

<h4 class="pdoc-member-header" id="IntegrationArgs-issueType">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-signalfx/blob/259fb9aba5c29d4cf535ca6c12ce9c3129fd56ab/sdk/nodejs/jira/integration.ts#L263">property <b>issueType</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>issueType: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</code></pre>

Issue type (for example, Story) for tickets that Jira creates for detector notifications. SignalFx validates issue types, so you must specify a type that's valid for the Jira project specified in `projectKey`.

<h4 class="pdoc-member-header" id="IntegrationArgs-name">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-signalfx/blob/259fb9aba5c29d4cf535ca6c12ce9c3129fd56ab/sdk/nodejs/jira/integration.ts#L267">property <b>name</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>name?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</code></pre>

Name of the integration.

<h4 class="pdoc-member-header" id="IntegrationArgs-password">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-signalfx/blob/259fb9aba5c29d4cf535ca6c12ce9c3129fd56ab/sdk/nodejs/jira/integration.ts#L271">property <b>password</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>password?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</code></pre>

Password used to authenticate the Jira integration.

<h4 class="pdoc-member-header" id="IntegrationArgs-projectKey">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-signalfx/blob/259fb9aba5c29d4cf535ca6c12ce9c3129fd56ab/sdk/nodejs/jira/integration.ts#L275">property <b>projectKey</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>projectKey: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</code></pre>

Jira key of an existing project. When Jira creates a new ticket for a detector notification, the ticket is assigned to this project.

<h4 class="pdoc-member-header" id="IntegrationArgs-userEmail">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-signalfx/blob/259fb9aba5c29d4cf535ca6c12ce9c3129fd56ab/sdk/nodejs/jira/integration.ts#L279">property <b>userEmail</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>userEmail?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</code></pre>

Email address used to authenticate the Jira integration.

<h4 class="pdoc-member-header" id="IntegrationArgs-username">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-signalfx/blob/259fb9aba5c29d4cf535ca6c12ce9c3129fd56ab/sdk/nodejs/jira/integration.ts#L283">property <b>username</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>username?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</code></pre>

User name used to authenticate the Jira integration.

<h3 class="pdoc-module-header" id="IntegrationState" data-link-title="IntegrationState">
    <a href="https://github.com/pulumi/pulumi-signalfx/blob/259fb9aba5c29d4cf535ca6c12ce9c3129fd56ab/sdk/nodejs/jira/integration.ts#L181">
        interface <strong>IntegrationState</strong>
    </a>
</h3>

<pre class="highlight"><code><span class='kr'>interface</span> <span class='nx'>IntegrationState</span></code></pre>

Input properties used for looking up and filtering Integration resources.

<h4 class="pdoc-member-header" id="IntegrationState-apiToken">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-signalfx/blob/259fb9aba5c29d4cf535ca6c12ce9c3129fd56ab/sdk/nodejs/jira/integration.ts#L185">property <b>apiToken</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>apiToken?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</code></pre>

The API token for the user email

<h4 class="pdoc-member-header" id="IntegrationState-assigneeDisplayName">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-signalfx/blob/259fb9aba5c29d4cf535ca6c12ce9c3129fd56ab/sdk/nodejs/jira/integration.ts#L189">property <b>assigneeDisplayName</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>assigneeDisplayName?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</code></pre>

Jira display name for the assignee.

<h4 class="pdoc-member-header" id="IntegrationState-assigneeName">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-signalfx/blob/259fb9aba5c29d4cf535ca6c12ce9c3129fd56ab/sdk/nodejs/jira/integration.ts#L193">property <b>assigneeName</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>assigneeName?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</code></pre>

Jira user name for the assignee.

<h4 class="pdoc-member-header" id="IntegrationState-authMethod">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-signalfx/blob/259fb9aba5c29d4cf535ca6c12ce9c3129fd56ab/sdk/nodejs/jira/integration.ts#L197">property <b>authMethod</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>authMethod?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</code></pre>

Authentication method used when creating the Jira integration. One of `EmailAndToken` (using `userEmail` and `apiToken`) or `UsernameAndPassword` (using `username` and `password`).

<h4 class="pdoc-member-header" id="IntegrationState-baseUrl">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-signalfx/blob/259fb9aba5c29d4cf535ca6c12ce9c3129fd56ab/sdk/nodejs/jira/integration.ts#L201">property <b>baseUrl</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>baseUrl?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</code></pre>

Base URL of the Jira instance that's integrated with SignalFx.

<h4 class="pdoc-member-header" id="IntegrationState-enabled">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-signalfx/blob/259fb9aba5c29d4cf535ca6c12ce9c3129fd56ab/sdk/nodejs/jira/integration.ts#L205">property <b>enabled</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>enabled?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean'>boolean</a></span>&gt;;</code></pre>

Whether the integration is enabled.

<h4 class="pdoc-member-header" id="IntegrationState-issueType">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-signalfx/blob/259fb9aba5c29d4cf535ca6c12ce9c3129fd56ab/sdk/nodejs/jira/integration.ts#L209">property <b>issueType</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>issueType?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</code></pre>

Issue type (for example, Story) for tickets that Jira creates for detector notifications. SignalFx validates issue types, so you must specify a type that's valid for the Jira project specified in `projectKey`.

<h4 class="pdoc-member-header" id="IntegrationState-name">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-signalfx/blob/259fb9aba5c29d4cf535ca6c12ce9c3129fd56ab/sdk/nodejs/jira/integration.ts#L213">property <b>name</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>name?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</code></pre>

Name of the integration.

<h4 class="pdoc-member-header" id="IntegrationState-password">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-signalfx/blob/259fb9aba5c29d4cf535ca6c12ce9c3129fd56ab/sdk/nodejs/jira/integration.ts#L217">property <b>password</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>password?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</code></pre>

Password used to authenticate the Jira integration.

<h4 class="pdoc-member-header" id="IntegrationState-projectKey">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-signalfx/blob/259fb9aba5c29d4cf535ca6c12ce9c3129fd56ab/sdk/nodejs/jira/integration.ts#L221">property <b>projectKey</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>projectKey?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</code></pre>

Jira key of an existing project. When Jira creates a new ticket for a detector notification, the ticket is assigned to this project.

<h4 class="pdoc-member-header" id="IntegrationState-userEmail">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-signalfx/blob/259fb9aba5c29d4cf535ca6c12ce9c3129fd56ab/sdk/nodejs/jira/integration.ts#L225">property <b>userEmail</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>userEmail?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</code></pre>

Email address used to authenticate the Jira integration.

<h4 class="pdoc-member-header" id="IntegrationState-username">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-signalfx/blob/259fb9aba5c29d4cf535ca6c12ce9c3129fd56ab/sdk/nodejs/jira/integration.ts#L229">property <b>username</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>username?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</code></pre>

User name used to authenticate the Jira integration.

