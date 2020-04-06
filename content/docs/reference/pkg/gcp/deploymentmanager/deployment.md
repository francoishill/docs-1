
---
title: "Deployment"
block_external_search_index: true
---

A collection of resources that are deployed and managed together using
a configuration file



> **Warning:** This resource is intended only to manage a Deployment resource,
and attempts to manage the Deployment's resources in the provider as well
will likely result in errors or unexpected behavior as the two tools
fight over ownership. We strongly discourage doing so unless you are an
experienced user of both tools.

In addition, due to limitations of the API, the provider will treat
deployments in preview as recreate-only for any update operation other
than actually deploying an in-preview deployment (i.e. `preview=true` to
`preview=false`).

> This content is derived from https://github.com/terraform-providers/terraform-provider-google/blob/master/website/docs/r/deployment_manager_deployment.html.markdown.



## Create a Deployment Resource

{{< chooser language "javascript,typescript,python,go,csharp" / >}}

{{% choosable language nodejs %}}
<div class="highlight"><pre class="chroma"><code class="language-typescript" data-lang="typescript"><span class="k">new </span><span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/gcp/deploymentmanager/#Deployment">Deployment</a></span><span class="p">(</span><span class="nx">name</span>: <span class="nx"><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string">string</a></span><span class="p">, </span><span class="nx">args</span>: <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/gcp/deploymentmanager/#DeploymentArgs">DeploymentArgs</a></span><span class="p">, </span><span class="nx">opts</span>?: <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/pulumi/#CustomResourceOptions">pulumi.CustomResourceOptions</a></span><span class="p">);</span></code></pre></div>
{{% /choosable %}}

{{% choosable language python %}}
<div class="highlight"><pre class="chroma"><code class="language-python" data-lang="python"><span class="k">def </span><span class="nf">Deployment</span><span class="p">(resource_name, opts=None, </span>create_policy=None<span class="p">, </span>delete_policy=None<span class="p">, </span>description=None<span class="p">, </span>labels=None<span class="p">, </span>name=None<span class="p">, </span>preview=None<span class="p">, </span>project=None<span class="p">, </span>target=None<span class="p">, __props__=None);</span></code></pre></div>
{{% /choosable %}}

{{% choosable language go %}}
<div class="highlight"><pre class="chroma"><code class="language-go" data-lang="go"><span class="k">func </span>NewDeployment<span class="p">(</span><span class="nx">ctx</span> *<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#Context">pulumi.Context</a></span><span class="p">, </span><span class="nx">name</span> <span class="nx"><a href="https://golang.org/pkg/builtin/#string">string</a></span><span class="p">, </span><span class="nx">args</span> <span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi-gcp/sdk/go/gcp/deploymentmanager?tab=doc#DeploymentArgs">DeploymentArgs</a></span><span class="p">, </span><span class="nx">opts</span> ...<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#ResourceOption">pulumi.ResourceOption</a></span><span class="p">) (*<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi-gcp/sdk/go/gcp/deploymentmanager?tab=doc#Deployment">Deployment</a></span>, error)</span></code></pre></div>
{{% /choosable %}}

{{% choosable language csharp %}}
<div class="highlight"><pre class="chroma"><code class="language-csharp" data-lang="csharp"><span class="k">public </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi.Gcp/Pulumi.Gcp.Deploymentmanager.Deployment.html">Deployment</a></span><span class="p">(</span><span class="nx"><a href="https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/built-in-types">string</a></span> <span class="nx">name<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi.Gcp/Pulumi.Gcp.DeploymentManager.DeploymentArgs.html">DeploymentArgs</a></span> <span class="nx">args<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi/Pulumi.CustomResourceOptions.html">CustomResourceOptions</a></span>? <span class="nx">opts = null<span class="p">)</span></code></pre></div>
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
        <span>Create<wbr>Policy</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Set the policy to use for creating new resources. Only used on create and update. Valid values are 'CREATE_OR_ACQUIRE'
(default) or 'ACQUIRE'. If set to 'ACQUIRE' and resources do not already exist, the deployment will fail. Note that
updating this field does not actually affect the deployment, just how it is updated.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Delete<wbr>Policy</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Set the policy to use for deleting new resources on update/delete. Valid values are 'DELETE' (default) or 'ABANDON'. If
'DELETE', resource is deleted after removal from Deployment Manager. If 'ABANDON', the resource is only removed from
Deployment Manager and is not actually deleted. Note that updating this field does not actually change the deployment,
just how it is updated.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Description</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Optional user-provided description of deployment.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Labels</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#deploymentlabel">List&lt;Deployment<wbr>Label<wbr>Args&gt;?</a></span>
    </dt>
    <dd>{{% md %}}Key-value pairs to apply to this labels.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Unique name for the deployment
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Preview</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool?</span>
    </dt>
    <dd>{{% md %}}If set to true, a deployment is created with "shell" resources that are not actually instantiated. This allows you to
preview a deployment. It can be updated to false to actually deploy with real resources. ~>**NOTE**: Deployment Manager
does not allow update of a deployment in preview (unless updating to preview=false). Thus, Terraform will force-recreate
deployments if either preview is updated to true or if other fields are updated while preview is true.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Project</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}The ID of the project in which the resource belongs.
If it is not provided, the provider project is used.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Target</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#deploymenttarget">Deployment<wbr>Target<wbr>Args</a></span>
    </dt>
    <dd>{{% md %}}Parameters that define your deployment, including the deployment configuration and relevant templates.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Create<wbr>Policy</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}Set the policy to use for creating new resources. Only used on create and update. Valid values are 'CREATE_OR_ACQUIRE'
(default) or 'ACQUIRE'. If set to 'ACQUIRE' and resources do not already exist, the deployment will fail. Note that
updating this field does not actually affect the deployment, just how it is updated.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Delete<wbr>Policy</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}Set the policy to use for deleting new resources on update/delete. Valid values are 'DELETE' (default) or 'ABANDON'. If
'DELETE', resource is deleted after removal from Deployment Manager. If 'ABANDON', the resource is only removed from
Deployment Manager and is not actually deleted. Note that updating this field does not actually change the deployment,
just how it is updated.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Description</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}Optional user-provided description of deployment.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Labels</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#deploymentlabel">[]Deployment<wbr>Label</a></span>
    </dt>
    <dd>{{% md %}}Key-value pairs to apply to this labels.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}Unique name for the deployment
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Preview</span>
        <span class="property-indicator"></span>
        <span class="property-type">*bool</span>
    </dt>
    <dd>{{% md %}}If set to true, a deployment is created with "shell" resources that are not actually instantiated. This allows you to
preview a deployment. It can be updated to false to actually deploy with real resources. ~>**NOTE**: Deployment Manager
does not allow update of a deployment in preview (unless updating to preview=false). Thus, Terraform will force-recreate
deployments if either preview is updated to true or if other fields are updated while preview is true.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Project</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}The ID of the project in which the resource belongs.
If it is not provided, the provider project is used.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Target</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#deploymenttarget">Deployment<wbr>Target</a></span>
    </dt>
    <dd>{{% md %}}Parameters that define your deployment, including the deployment configuration and relevant templates.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>create<wbr>Policy</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Set the policy to use for creating new resources. Only used on create and update. Valid values are 'CREATE_OR_ACQUIRE'
(default) or 'ACQUIRE'. If set to 'ACQUIRE' and resources do not already exist, the deployment will fail. Note that
updating this field does not actually affect the deployment, just how it is updated.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>delete<wbr>Policy</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Set the policy to use for deleting new resources on update/delete. Valid values are 'DELETE' (default) or 'ABANDON'. If
'DELETE', resource is deleted after removal from Deployment Manager. If 'ABANDON', the resource is only removed from
Deployment Manager and is not actually deleted. Note that updating this field does not actually change the deployment,
just how it is updated.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>description</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Optional user-provided description of deployment.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>labels</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#deploymentlabel">Deployment<wbr>Label[]?</a></span>
    </dt>
    <dd>{{% md %}}Key-value pairs to apply to this labels.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Unique name for the deployment
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>preview</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean?</span>
    </dt>
    <dd>{{% md %}}If set to true, a deployment is created with "shell" resources that are not actually instantiated. This allows you to
preview a deployment. It can be updated to false to actually deploy with real resources. ~>**NOTE**: Deployment Manager
does not allow update of a deployment in preview (unless updating to preview=false). Thus, Terraform will force-recreate
deployments if either preview is updated to true or if other fields are updated while preview is true.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>project</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}The ID of the project in which the resource belongs.
If it is not provided, the provider project is used.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>target</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#deploymenttarget">Deployment<wbr>Target</a></span>
    </dt>
    <dd>{{% md %}}Parameters that define your deployment, including the deployment configuration and relevant templates.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>create_<wbr>policy</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Set the policy to use for creating new resources. Only used on create and update. Valid values are 'CREATE_OR_ACQUIRE'
(default) or 'ACQUIRE'. If set to 'ACQUIRE' and resources do not already exist, the deployment will fail. Note that
updating this field does not actually affect the deployment, just how it is updated.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>delete_<wbr>policy</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Set the policy to use for deleting new resources on update/delete. Valid values are 'DELETE' (default) or 'ABANDON'. If
'DELETE', resource is deleted after removal from Deployment Manager. If 'ABANDON', the resource is only removed from
Deployment Manager and is not actually deleted. Note that updating this field does not actually change the deployment,
just how it is updated.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>description</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Optional user-provided description of deployment.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>labels</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#deploymentlabel">List[Deployment<wbr>Label]</a></span>
    </dt>
    <dd>{{% md %}}Key-value pairs to apply to this labels.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Unique name for the deployment
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>preview</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}If set to true, a deployment is created with "shell" resources that are not actually instantiated. This allows you to
preview a deployment. It can be updated to false to actually deploy with real resources. ~>**NOTE**: Deployment Manager
does not allow update of a deployment in preview (unless updating to preview=false). Thus, Terraform will force-recreate
deployments if either preview is updated to true or if other fields are updated while preview is true.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>project</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The ID of the project in which the resource belongs.
If it is not provided, the provider project is used.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>target</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#deploymenttarget">Dict[Deployment<wbr>Target]</a></span>
    </dt>
    <dd>{{% md %}}Parameters that define your deployment, including the deployment configuration and relevant templates.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}







## Deployment Output Properties

The following output properties are available:




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-"
            title="">
        <span>Create<wbr>Policy</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Set the policy to use for creating new resources. Only used on create and update. Valid values are 'CREATE_OR_ACQUIRE'
(default) or 'ACQUIRE'. If set to 'ACQUIRE' and resources do not already exist, the deployment will fail. Note that
updating this field does not actually affect the deployment, just how it is updated.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Delete<wbr>Policy</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Set the policy to use for deleting new resources on update/delete. Valid values are 'DELETE' (default) or 'ABANDON'. If
'DELETE', resource is deleted after removal from Deployment Manager. If 'ABANDON', the resource is only removed from
Deployment Manager and is not actually deleted. Note that updating this field does not actually change the deployment,
just how it is updated.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Deployment<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Unique identifier for deployment. Output only.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Description</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Optional user-provided description of deployment.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Labels</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#deploymentlabel">List&lt;Deployment<wbr>Label&gt;?</a></span>
    </dt>
    <dd>{{% md %}}Key-value pairs to apply to this labels.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Manifest</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Output only. URL of the manifest representing the last manifest that was successfully deployed.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Unique name for the deployment
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Preview</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool?</span>
    </dt>
    <dd>{{% md %}}If set to true, a deployment is created with "shell" resources that are not actually instantiated. This allows you to
preview a deployment. It can be updated to false to actually deploy with real resources. ~>**NOTE**: Deployment Manager
does not allow update of a deployment in preview (unless updating to preview=false). Thus, Terraform will force-recreate
deployments if either preview is updated to true or if other fields are updated while preview is true.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Project</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The ID of the project in which the resource belongs.
If it is not provided, the provider project is used.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Self<wbr>Link</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Output only. Server defined URL for the resource.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Target</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#deploymenttarget">Deployment<wbr>Target</a></span>
    </dt>
    <dd>{{% md %}}Parameters that define your deployment, including the deployment configuration and relevant templates.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-"
            title="">
        <span>Create<wbr>Policy</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}Set the policy to use for creating new resources. Only used on create and update. Valid values are 'CREATE_OR_ACQUIRE'
(default) or 'ACQUIRE'. If set to 'ACQUIRE' and resources do not already exist, the deployment will fail. Note that
updating this field does not actually affect the deployment, just how it is updated.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Delete<wbr>Policy</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}Set the policy to use for deleting new resources on update/delete. Valid values are 'DELETE' (default) or 'ABANDON'. If
'DELETE', resource is deleted after removal from Deployment Manager. If 'ABANDON', the resource is only removed from
Deployment Manager and is not actually deleted. Note that updating this field does not actually change the deployment,
just how it is updated.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Deployment<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Unique identifier for deployment. Output only.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Description</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}Optional user-provided description of deployment.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Labels</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#deploymentlabel">[]Deployment<wbr>Label</a></span>
    </dt>
    <dd>{{% md %}}Key-value pairs to apply to this labels.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Manifest</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Output only. URL of the manifest representing the last manifest that was successfully deployed.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Unique name for the deployment
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Preview</span>
        <span class="property-indicator"></span>
        <span class="property-type">*bool</span>
    </dt>
    <dd>{{% md %}}If set to true, a deployment is created with "shell" resources that are not actually instantiated. This allows you to
preview a deployment. It can be updated to false to actually deploy with real resources. ~>**NOTE**: Deployment Manager
does not allow update of a deployment in preview (unless updating to preview=false). Thus, Terraform will force-recreate
deployments if either preview is updated to true or if other fields are updated while preview is true.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Project</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The ID of the project in which the resource belongs.
If it is not provided, the provider project is used.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Self<wbr>Link</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Output only. Server defined URL for the resource.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Target</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#deploymenttarget">Deployment<wbr>Target</a></span>
    </dt>
    <dd>{{% md %}}Parameters that define your deployment, including the deployment configuration and relevant templates.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-"
            title="">
        <span>create<wbr>Policy</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Set the policy to use for creating new resources. Only used on create and update. Valid values are 'CREATE_OR_ACQUIRE'
(default) or 'ACQUIRE'. If set to 'ACQUIRE' and resources do not already exist, the deployment will fail. Note that
updating this field does not actually affect the deployment, just how it is updated.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>delete<wbr>Policy</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Set the policy to use for deleting new resources on update/delete. Valid values are 'DELETE' (default) or 'ABANDON'. If
'DELETE', resource is deleted after removal from Deployment Manager. If 'ABANDON', the resource is only removed from
Deployment Manager and is not actually deleted. Note that updating this field does not actually change the deployment,
just how it is updated.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>deployment<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Unique identifier for deployment. Output only.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>description</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Optional user-provided description of deployment.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>labels</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#deploymentlabel">Deployment<wbr>Label[]?</a></span>
    </dt>
    <dd>{{% md %}}Key-value pairs to apply to this labels.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>manifest</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Output only. URL of the manifest representing the last manifest that was successfully deployed.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Unique name for the deployment
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>preview</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean?</span>
    </dt>
    <dd>{{% md %}}If set to true, a deployment is created with "shell" resources that are not actually instantiated. This allows you to
preview a deployment. It can be updated to false to actually deploy with real resources. ~>**NOTE**: Deployment Manager
does not allow update of a deployment in preview (unless updating to preview=false). Thus, Terraform will force-recreate
deployments if either preview is updated to true or if other fields are updated while preview is true.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>project</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The ID of the project in which the resource belongs.
If it is not provided, the provider project is used.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>self<wbr>Link</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Output only. Server defined URL for the resource.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>target</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#deploymenttarget">Deployment<wbr>Target</a></span>
    </dt>
    <dd>{{% md %}}Parameters that define your deployment, including the deployment configuration and relevant templates.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-"
            title="">
        <span>create_<wbr>policy</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Set the policy to use for creating new resources. Only used on create and update. Valid values are 'CREATE_OR_ACQUIRE'
(default) or 'ACQUIRE'. If set to 'ACQUIRE' and resources do not already exist, the deployment will fail. Note that
updating this field does not actually affect the deployment, just how it is updated.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>delete_<wbr>policy</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Set the policy to use for deleting new resources on update/delete. Valid values are 'DELETE' (default) or 'ABANDON'. If
'DELETE', resource is deleted after removal from Deployment Manager. If 'ABANDON', the resource is only removed from
Deployment Manager and is not actually deleted. Note that updating this field does not actually change the deployment,
just how it is updated.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>deployment_<wbr>id</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Unique identifier for deployment. Output only.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>description</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Optional user-provided description of deployment.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>labels</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#deploymentlabel">List[Deployment<wbr>Label]</a></span>
    </dt>
    <dd>{{% md %}}Key-value pairs to apply to this labels.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>manifest</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Output only. URL of the manifest representing the last manifest that was successfully deployed.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Unique name for the deployment
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>preview</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}If set to true, a deployment is created with "shell" resources that are not actually instantiated. This allows you to
preview a deployment. It can be updated to false to actually deploy with real resources. ~>**NOTE**: Deployment Manager
does not allow update of a deployment in preview (unless updating to preview=false). Thus, Terraform will force-recreate
deployments if either preview is updated to true or if other fields are updated while preview is true.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>project</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The ID of the project in which the resource belongs.
If it is not provided, the provider project is used.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>self_<wbr>link</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Output only. Server defined URL for the resource.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>target</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#deploymenttarget">Dict[Deployment<wbr>Target]</a></span>
    </dt>
    <dd>{{% md %}}Parameters that define your deployment, including the deployment configuration and relevant templates.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}








## Look up an Existing Deployment Resource

Get an existing Deployment resource's state with the given name, ID, and optional extra properties used to qualify the lookup.

{{< chooser language "javascript,typescript,python,go,csharp  " / >}}

{{% choosable language nodejs %}}
<div class="highlight"><pre class="chroma"><code class="language-typescript" data-lang="typescript"><span class="k">public static </span><span class="nf">get</span><span class="p">(</span><span class="nx">name</span>: <span class="nx"><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string">string</a></span><span class="p">, </span><span class="nx">id</span>: <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/pulumi/#ID">Input&lt;ID&gt;</a></span><span class="p">, </span><span class="nx">state</span>?: <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/gcp/deploymentmanager/#DeploymentState">DeploymentState</a></span><span class="p">, </span><span class="nx">opts</span>?: <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/pulumi/#CustomResourceOptions">CustomResourceOptions</a></span><span class="p">): </span><span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/gcp/deploymentmanager/#Deployment">Deployment</a></span></code></pre></div>
{{% /choosable %}}

{{% choosable language python %}}
<div class="highlight"><pre class="chroma"><code class="language-python" data-lang="python"><span class="k">static </span><span class="nf">get</span><span class="p">(resource_name, id, opts=None, </span>create_policy=None<span class="p">, </span>delete_policy=None<span class="p">, </span>deployment_id=None<span class="p">, </span>description=None<span class="p">, </span>labels=None<span class="p">, </span>manifest=None<span class="p">, </span>name=None<span class="p">, </span>preview=None<span class="p">, </span>project=None<span class="p">, </span>self_link=None<span class="p">, </span>target=None<span class="p">, __props__=None);</span></code></pre></div>
{{% /choosable %}}

{{% choosable language go %}}
<div class="highlight"><pre class="chroma"><code class="language-go" data-lang="go"><span class="k">func </span>GetDeployment<span class="p">(</span><span class="nx">ctx</span> *<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#Context">Context</a></span><span class="p">, </span><span class="nx">name</span> <span class="nx"><a href="https://golang.org/pkg/builtin/#string">string</a></span><span class="p">, </span><span class="nx">id</span> <span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#IDInput">IDInput</a></span><span class="p">, </span><span class="nx">state</span> *<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi-gcp/sdk/go/gcp/deploymentmanager?tab=doc#DeploymentState">DeploymentState</a></span><span class="p">, </span><span class="nx">opts</span> ...<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#ResourceOption">ResourceOption</a></span><span class="p">) (*<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi-gcp/sdk/go/gcp/deploymentmanager?tab=doc#Deployment">Deployment</a></span>, error)</span></code></pre></div>
{{% /choosable %}}

{{% choosable language csharp %}}
<div class="highlight"><pre class="chroma"><code class="language-csharp" data-lang="csharp"><span class="k">public static </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi.Gcp/Pulumi.Gcp.Deploymentmanager.Deployment.html">Deployment</a></span><span class="nf"> Get</span><span class="p">(</span><span class="nx"><a href="https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/built-in-types">string</a></span> <span class="nx">name<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi/Pulumi.Input.html">Input&lt;string&gt;</a></span> <span class="nx">id<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi.Gcp/Pulumi.Gcp.Deploymentmanager.DeploymentState.html">DeploymentState</a></span>? <span class="nx">state<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi/Pulumi.CustomResourceOptions.html">CustomResourceOptions</a></span>? <span class="nx">opts = null<span class="p">)</span></code></pre></div>
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
        <span>Create<wbr>Policy</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Set the policy to use for creating new resources. Only used on create and update. Valid values are 'CREATE_OR_ACQUIRE'
(default) or 'ACQUIRE'. If set to 'ACQUIRE' and resources do not already exist, the deployment will fail. Note that
updating this field does not actually affect the deployment, just how it is updated.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Delete<wbr>Policy</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Set the policy to use for deleting new resources on update/delete. Valid values are 'DELETE' (default) or 'ABANDON'. If
'DELETE', resource is deleted after removal from Deployment Manager. If 'ABANDON', the resource is only removed from
Deployment Manager and is not actually deleted. Note that updating this field does not actually change the deployment,
just how it is updated.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Deployment<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Unique identifier for deployment. Output only.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Description</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Optional user-provided description of deployment.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Labels</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#deploymentlabel">List&lt;Deployment<wbr>Label<wbr>Args&gt;?</a></span>
    </dt>
    <dd>{{% md %}}Key-value pairs to apply to this labels.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Manifest</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Output only. URL of the manifest representing the last manifest that was successfully deployed.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Unique name for the deployment
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Preview</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool?</span>
    </dt>
    <dd>{{% md %}}If set to true, a deployment is created with "shell" resources that are not actually instantiated. This allows you to
preview a deployment. It can be updated to false to actually deploy with real resources. ~>**NOTE**: Deployment Manager
does not allow update of a deployment in preview (unless updating to preview=false). Thus, Terraform will force-recreate
deployments if either preview is updated to true or if other fields are updated while preview is true.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Project</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}The ID of the project in which the resource belongs.
If it is not provided, the provider project is used.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Self<wbr>Link</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Output only. Server defined URL for the resource.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Target</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#deploymenttarget">Deployment<wbr>Target<wbr>Args?</a></span>
    </dt>
    <dd>{{% md %}}Parameters that define your deployment, including the deployment configuration and relevant templates.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Create<wbr>Policy</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}Set the policy to use for creating new resources. Only used on create and update. Valid values are 'CREATE_OR_ACQUIRE'
(default) or 'ACQUIRE'. If set to 'ACQUIRE' and resources do not already exist, the deployment will fail. Note that
updating this field does not actually affect the deployment, just how it is updated.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Delete<wbr>Policy</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}Set the policy to use for deleting new resources on update/delete. Valid values are 'DELETE' (default) or 'ABANDON'. If
'DELETE', resource is deleted after removal from Deployment Manager. If 'ABANDON', the resource is only removed from
Deployment Manager and is not actually deleted. Note that updating this field does not actually change the deployment,
just how it is updated.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Deployment<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}Unique identifier for deployment. Output only.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Description</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}Optional user-provided description of deployment.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Labels</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#deploymentlabel">[]Deployment<wbr>Label</a></span>
    </dt>
    <dd>{{% md %}}Key-value pairs to apply to this labels.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Manifest</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}Output only. URL of the manifest representing the last manifest that was successfully deployed.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}Unique name for the deployment
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Preview</span>
        <span class="property-indicator"></span>
        <span class="property-type">*bool</span>
    </dt>
    <dd>{{% md %}}If set to true, a deployment is created with "shell" resources that are not actually instantiated. This allows you to
preview a deployment. It can be updated to false to actually deploy with real resources. ~>**NOTE**: Deployment Manager
does not allow update of a deployment in preview (unless updating to preview=false). Thus, Terraform will force-recreate
deployments if either preview is updated to true or if other fields are updated while preview is true.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Project</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}The ID of the project in which the resource belongs.
If it is not provided, the provider project is used.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Self<wbr>Link</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}Output only. Server defined URL for the resource.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Target</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#deploymenttarget">*Deployment<wbr>Target</a></span>
    </dt>
    <dd>{{% md %}}Parameters that define your deployment, including the deployment configuration and relevant templates.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>create<wbr>Policy</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Set the policy to use for creating new resources. Only used on create and update. Valid values are 'CREATE_OR_ACQUIRE'
(default) or 'ACQUIRE'. If set to 'ACQUIRE' and resources do not already exist, the deployment will fail. Note that
updating this field does not actually affect the deployment, just how it is updated.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>delete<wbr>Policy</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Set the policy to use for deleting new resources on update/delete. Valid values are 'DELETE' (default) or 'ABANDON'. If
'DELETE', resource is deleted after removal from Deployment Manager. If 'ABANDON', the resource is only removed from
Deployment Manager and is not actually deleted. Note that updating this field does not actually change the deployment,
just how it is updated.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>deployment<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Unique identifier for deployment. Output only.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>description</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Optional user-provided description of deployment.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>labels</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#deploymentlabel">Deployment<wbr>Label[]?</a></span>
    </dt>
    <dd>{{% md %}}Key-value pairs to apply to this labels.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>manifest</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Output only. URL of the manifest representing the last manifest that was successfully deployed.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Unique name for the deployment
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>preview</span>
        <span class="property-indicator"></span>
        <span class="property-type">boolean?</span>
    </dt>
    <dd>{{% md %}}If set to true, a deployment is created with "shell" resources that are not actually instantiated. This allows you to
preview a deployment. It can be updated to false to actually deploy with real resources. ~>**NOTE**: Deployment Manager
does not allow update of a deployment in preview (unless updating to preview=false). Thus, Terraform will force-recreate
deployments if either preview is updated to true or if other fields are updated while preview is true.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>project</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}The ID of the project in which the resource belongs.
If it is not provided, the provider project is used.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>self<wbr>Link</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Output only. Server defined URL for the resource.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>target</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#deploymenttarget">Deployment<wbr>Target?</a></span>
    </dt>
    <dd>{{% md %}}Parameters that define your deployment, including the deployment configuration and relevant templates.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>create_<wbr>policy</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Set the policy to use for creating new resources. Only used on create and update. Valid values are 'CREATE_OR_ACQUIRE'
(default) or 'ACQUIRE'. If set to 'ACQUIRE' and resources do not already exist, the deployment will fail. Note that
updating this field does not actually affect the deployment, just how it is updated.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>delete_<wbr>policy</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Set the policy to use for deleting new resources on update/delete. Valid values are 'DELETE' (default) or 'ABANDON'. If
'DELETE', resource is deleted after removal from Deployment Manager. If 'ABANDON', the resource is only removed from
Deployment Manager and is not actually deleted. Note that updating this field does not actually change the deployment,
just how it is updated.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>deployment_<wbr>id</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Unique identifier for deployment. Output only.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>description</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Optional user-provided description of deployment.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>labels</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#deploymentlabel">List[Deployment<wbr>Label]</a></span>
    </dt>
    <dd>{{% md %}}Key-value pairs to apply to this labels.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>manifest</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Output only. URL of the manifest representing the last manifest that was successfully deployed.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Unique name for the deployment
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>preview</span>
        <span class="property-indicator"></span>
        <span class="property-type">bool</span>
    </dt>
    <dd>{{% md %}}If set to true, a deployment is created with "shell" resources that are not actually instantiated. This allows you to
preview a deployment. It can be updated to false to actually deploy with real resources. ~>**NOTE**: Deployment Manager
does not allow update of a deployment in preview (unless updating to preview=false). Thus, Terraform will force-recreate
deployments if either preview is updated to true or if other fields are updated while preview is true.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>project</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The ID of the project in which the resource belongs.
If it is not provided, the provider project is used.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>self_<wbr>link</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Output only. Server defined URL for the resource.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>target</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#deploymenttarget">Dict[Deployment<wbr>Target]</a></span>
    </dt>
    <dd>{{% md %}}Parameters that define your deployment, including the deployment configuration and relevant templates.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}










## Supporting Types

<h4>Deployment<wbr>Label</h4>
{{% choosable language nodejs %}}
> See the <a href="/docs/reference/pkg/nodejs/pulumi/gcp/types/input/#DeploymentLabel">input</a> and <a href="/docs/reference/pkg/nodejs/pulumi/gcp/types/output/#DeploymentLabel">output</a> API doc for this type.
{{% /choosable %}}

{{% choosable language go %}}
> See the <a href="https://pkg.go.dev/github.com/pulumi/pulumi-gcp/sdk/go/gcp/deploymentmanager?tab=doc#DeploymentLabelArgs">input</a> and <a href="https://pkg.go.dev/github.com/pulumi/pulumi-gcp/sdk/go/gcp/deploymentmanager?tab=doc#DeploymentLabelOutput">output</a> API doc for this type.
{{% /choosable %}}




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Key</span>
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
        <span>Key</span>
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
        <span>key</span>
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
        <span>key</span>
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





<h4>Deployment<wbr>Target</h4>
{{% choosable language nodejs %}}
> See the <a href="/docs/reference/pkg/nodejs/pulumi/gcp/types/input/#DeploymentTarget">input</a> and <a href="/docs/reference/pkg/nodejs/pulumi/gcp/types/output/#DeploymentTarget">output</a> API doc for this type.
{{% /choosable %}}

{{% choosable language go %}}
> See the <a href="https://pkg.go.dev/github.com/pulumi/pulumi-gcp/sdk/go/gcp/deploymentmanager?tab=doc#DeploymentTargetArgs">input</a> and <a href="https://pkg.go.dev/github.com/pulumi/pulumi-gcp/sdk/go/gcp/deploymentmanager?tab=doc#DeploymentTargetOutput">output</a> API doc for this type.
{{% /choosable %}}




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>Config</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#deploymenttargetconfig">Deployment<wbr>Target<wbr>Config<wbr>Args</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Imports</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#deploymenttargetimport">List&lt;Deployment<wbr>Target<wbr>Import<wbr>Args&gt;?</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>Config</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#deploymenttargetconfig">Deployment<wbr>Target<wbr>Config</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Imports</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#deploymenttargetimport">[]Deployment<wbr>Target<wbr>Import</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>config</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#deploymenttargetconfig">Deployment<wbr>Target<wbr>Config</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>imports</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#deploymenttargetimport">Deployment<wbr>Target<wbr>Import[]?</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>config</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#deploymenttargetconfig">Dict[Deployment<wbr>Target<wbr>Config]</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>imports</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#deploymenttargetimport">List[Deployment<wbr>Target<wbr>Import]</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

</dl>
{{% /choosable %}}





<h4>Deployment<wbr>Target<wbr>Config</h4>
{{% choosable language nodejs %}}
> See the <a href="/docs/reference/pkg/nodejs/pulumi/gcp/types/input/#DeploymentTargetConfig">input</a> and <a href="/docs/reference/pkg/nodejs/pulumi/gcp/types/output/#DeploymentTargetConfig">output</a> API doc for this type.
{{% /choosable %}}

{{% choosable language go %}}
> See the <a href="https://pkg.go.dev/github.com/pulumi/pulumi-gcp/sdk/go/gcp/deploymentmanager?tab=doc#DeploymentTargetConfigArgs">input</a> and <a href="https://pkg.go.dev/github.com/pulumi/pulumi-gcp/sdk/go/gcp/deploymentmanager?tab=doc#DeploymentTargetConfigOutput">output</a> API doc for this type.
{{% /choosable %}}




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>Content</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>Content</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>content</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>content</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

</dl>
{{% /choosable %}}





<h4>Deployment<wbr>Target<wbr>Import</h4>
{{% choosable language nodejs %}}
> See the <a href="/docs/reference/pkg/nodejs/pulumi/gcp/types/input/#DeploymentTargetImport">input</a> and <a href="/docs/reference/pkg/nodejs/pulumi/gcp/types/output/#DeploymentTargetImport">output</a> API doc for this type.
{{% /choosable %}}

{{% choosable language go %}}
> See the <a href="https://pkg.go.dev/github.com/pulumi/pulumi-gcp/sdk/go/gcp/deploymentmanager?tab=doc#DeploymentTargetImportArgs">input</a> and <a href="https://pkg.go.dev/github.com/pulumi/pulumi-gcp/sdk/go/gcp/deploymentmanager?tab=doc#DeploymentTargetImportOutput">output</a> API doc for this type.
{{% /choosable %}}




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Content</span>
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
    <dd>{{% md %}}{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Content</span>
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
    <dd>{{% md %}}{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>content</span>
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
    <dd>{{% md %}}{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>content</span>
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
    <dd>{{% md %}}{{% /md %}}</dd>

</dl>
{{% /choosable %}}








<h3>Package Details</h3>
<dl class="package-details">
	<dt>Repository</dt>
	<dd><a href="https://github.com/pulumi/pulumi-gcp">https://github.com/pulumi/pulumi-gcp</a></dd>
	<dt>License</dt>
	<dd>Apache-2.0</dd></dl>