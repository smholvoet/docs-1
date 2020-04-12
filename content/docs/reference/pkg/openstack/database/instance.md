
---
title: "Instance"
block_external_search_index: true
---



Manages a V1 DB instance resource within OpenStack.

## Example Usage

### Instance

```typescript
import * as pulumi from "@pulumi/pulumi";
import * as openstack from "@pulumi/openstack";

const test = new openstack.database.Instance("test", {
    datastore: {
        type: "mysql",
        version: "mysql-5.7",
    },
    flavorId: "31792d21-c355-4587-9290-56c1ed0ca376",
    networks: [{
        uuid: "c0612505-caf2-4fb0-b7cb-56a0240a2b12",
    }],
    region: "region-test",
    size: 8,
});
```

> This content is derived from https://github.com/terraform-providers/terraform-provider-openstack/blob/master/website/docs/r/db_instance_v1.html.markdown.



## Create a Instance Resource

{{< chooser language "javascript,typescript,python,go,csharp" / >}}

{{% choosable language nodejs %}}
<div class="highlight"><pre class="chroma"><code class="language-typescript" data-lang="typescript"><span class="k">new </span><span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/openstack/database/#Instance">Instance</a></span><span class="p">(</span><span class="nx">name</span>: <span class="nx"><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string">string</a></span><span class="p">, </span><span class="nx">args</span>: <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/openstack/database/#InstanceArgs">InstanceArgs</a></span><span class="p">, </span><span class="nx">opts</span>?: <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/pulumi/#CustomResourceOptions">pulumi.CustomResourceOptions</a></span><span class="p">);</span></code></pre></div>
{{% /choosable %}}

{{% choosable language python %}}
<div class="highlight"><pre class="chroma"><code class="language-python" data-lang="python"><span class="k">def </span><span class="nf">Instance</span><span class="p">(resource_name, opts=None, </span>configuration_id=None<span class="p">, </span>databases=None<span class="p">, </span>datastore=None<span class="p">, </span>flavor_id=None<span class="p">, </span>name=None<span class="p">, </span>networks=None<span class="p">, </span>region=None<span class="p">, </span>size=None<span class="p">, </span>users=None<span class="p">, __props__=None);</span></code></pre></div>
{{% /choosable %}}

{{% choosable language go %}}
<div class="highlight"><pre class="chroma"><code class="language-go" data-lang="go"><span class="k">func </span>NewInstance<span class="p">(</span><span class="nx">ctx</span> *<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#Context">pulumi.Context</a></span><span class="p">, </span><span class="nx">name</span> <span class="nx"><a href="https://golang.org/pkg/builtin/#string">string</a></span><span class="p">, </span><span class="nx">args</span> <span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi-openstack/sdk/go/openstack/database?tab=doc#InstanceArgs">InstanceArgs</a></span><span class="p">, </span><span class="nx">opts</span> ...<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#ResourceOption">pulumi.ResourceOption</a></span><span class="p">) (*<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi-openstack/sdk/go/openstack/database?tab=doc#Instance">Instance</a></span>, error)</span></code></pre></div>
{{% /choosable %}}

{{% choosable language csharp %}}
<div class="highlight"><pre class="chroma"><code class="language-csharp" data-lang="csharp"><span class="k">public </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi.Openstack/Pulumi.Openstack.Database.Instance.html">Instance</a></span><span class="p">(</span><span class="nx"><a href="https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/built-in-types">string</a></span> <span class="nx">name<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi.Openstack/Pulumi.Openstack.Database.InstanceArgs.html">InstanceArgs</a></span> <span class="nx">args<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi/Pulumi.CustomResourceOptions.html">CustomResourceOptions</a></span>? <span class="nx">opts = null<span class="p">)</span></code></pre></div>
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
        <span>Configuration<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Configuration ID to be attached to the instance. Database instance
will be rebooted when configuration is detached.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Databases</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#instancedatabase">List&lt;Instance<wbr>Database<wbr>Args&gt;?</a></span>
    </dt>
    <dd>{{% md %}}An array of database name, charset and collate. The database
object structure is documented below.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Datastore</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#instancedatastore">Instance<wbr>Datastore<wbr>Args</a></span>
    </dt>
    <dd>{{% md %}}An array of database engine type and version. The datastore
object structure is documented below. Changing this creates a new instance.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Flavor<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}The flavor ID of the desired flavor for the instance.
Changing this creates new instance.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Database to be created on new instance. Changing this creates a
new instance.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Networks</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#instancenetwork">List&lt;Instance<wbr>Network<wbr>Args&gt;?</a></span>
    </dt>
    <dd>{{% md %}}An array of one or more networks to attach to the
instance. The network object structure is documented below. Changing this
creates a new instance.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Region</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}The region in which to create the db instance. Changing this
creates a new instance.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Size</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}Specifies the volume size in GB. Changing this creates new instance.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Users</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#instanceuser">List&lt;Instance<wbr>User<wbr>Args&gt;?</a></span>
    </dt>
    <dd>{{% md %}}An array of username, password, host and databases. The user
object structure is documented below.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Configuration<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}Configuration ID to be attached to the instance. Database instance
will be rebooted when configuration is detached.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Databases</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#instancedatabase">[]Instance<wbr>Database</a></span>
    </dt>
    <dd>{{% md %}}An array of database name, charset and collate. The database
object structure is documented below.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Datastore</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#instancedatastore">Instance<wbr>Datastore</a></span>
    </dt>
    <dd>{{% md %}}An array of database engine type and version. The datastore
object structure is documented below. Changing this creates a new instance.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Flavor<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}The flavor ID of the desired flavor for the instance.
Changing this creates new instance.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}Database to be created on new instance. Changing this creates a
new instance.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Networks</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#instancenetwork">[]Instance<wbr>Network</a></span>
    </dt>
    <dd>{{% md %}}An array of one or more networks to attach to the
instance. The network object structure is documented below. Changing this
creates a new instance.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Region</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}The region in which to create the db instance. Changing this
creates a new instance.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Size</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}Specifies the volume size in GB. Changing this creates new instance.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Users</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#instanceuser">[]Instance<wbr>User</a></span>
    </dt>
    <dd>{{% md %}}An array of username, password, host and databases. The user
object structure is documented below.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>configuration<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Configuration ID to be attached to the instance. Database instance
will be rebooted when configuration is detached.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>databases</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#instancedatabase">Instance<wbr>Database[]?</a></span>
    </dt>
    <dd>{{% md %}}An array of database name, charset and collate. The database
object structure is documented below.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>datastore</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#instancedatastore">Instance<wbr>Datastore</a></span>
    </dt>
    <dd>{{% md %}}An array of database engine type and version. The datastore
object structure is documented below. Changing this creates a new instance.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>flavor<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}The flavor ID of the desired flavor for the instance.
Changing this creates new instance.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Database to be created on new instance. Changing this creates a
new instance.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>networks</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#instancenetwork">Instance<wbr>Network[]?</a></span>
    </dt>
    <dd>{{% md %}}An array of one or more networks to attach to the
instance. The network object structure is documented below. Changing this
creates a new instance.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>region</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}The region in which to create the db instance. Changing this
creates a new instance.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>size</span>
        <span class="property-indicator"></span>
        <span class="property-type">number</span>
    </dt>
    <dd>{{% md %}}Specifies the volume size in GB. Changing this creates new instance.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>users</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#instanceuser">Instance<wbr>User[]?</a></span>
    </dt>
    <dd>{{% md %}}An array of username, password, host and databases. The user
object structure is documented below.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>configuration_<wbr>id</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Configuration ID to be attached to the instance. Database instance
will be rebooted when configuration is detached.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>databases</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#instancedatabase">List[Instance<wbr>Database]</a></span>
    </dt>
    <dd>{{% md %}}An array of database name, charset and collate. The database
object structure is documented below.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>datastore</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#instancedatastore">Dict[Instance<wbr>Datastore]</a></span>
    </dt>
    <dd>{{% md %}}An array of database engine type and version. The datastore
object structure is documented below. Changing this creates a new instance.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>flavor_<wbr>id</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The flavor ID of the desired flavor for the instance.
Changing this creates new instance.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Database to be created on new instance. Changing this creates a
new instance.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>networks</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#instancenetwork">List[Instance<wbr>Network]</a></span>
    </dt>
    <dd>{{% md %}}An array of one or more networks to attach to the
instance. The network object structure is documented below. Changing this
creates a new instance.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>region</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The region in which to create the db instance. Changing this
creates a new instance.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>size</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}Specifies the volume size in GB. Changing this creates new instance.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>users</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#instanceuser">List[Instance<wbr>User]</a></span>
    </dt>
    <dd>{{% md %}}An array of username, password, host and databases. The user
object structure is documented below.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}







## Instance Output Properties

The following output properties are available:




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-"
            title="">
        <span>Configuration<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Configuration ID to be attached to the instance. Database instance
will be rebooted when configuration is detached.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Databases</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#instancedatabase">List&lt;Instance<wbr>Database&gt;?</a></span>
    </dt>
    <dd>{{% md %}}An array of database name, charset and collate. The database
object structure is documented below.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Datastore</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#instancedatastore">Instance<wbr>Datastore</a></span>
    </dt>
    <dd>{{% md %}}An array of database engine type and version. The datastore
object structure is documented below. Changing this creates a new instance.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Flavor<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The flavor ID of the desired flavor for the instance.
Changing this creates new instance.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Database to be created on new instance. Changing this creates a
new instance.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Networks</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#instancenetwork">List&lt;Instance<wbr>Network&gt;?</a></span>
    </dt>
    <dd>{{% md %}}An array of one or more networks to attach to the
instance. The network object structure is documented below. Changing this
creates a new instance.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Region</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The region in which to create the db instance. Changing this
creates a new instance.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Size</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}Specifies the volume size in GB. Changing this creates new instance.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Users</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#instanceuser">List&lt;Instance<wbr>User&gt;?</a></span>
    </dt>
    <dd>{{% md %}}An array of username, password, host and databases. The user
object structure is documented below.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-"
            title="">
        <span>Configuration<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}Configuration ID to be attached to the instance. Database instance
will be rebooted when configuration is detached.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Databases</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#instancedatabase">[]Instance<wbr>Database</a></span>
    </dt>
    <dd>{{% md %}}An array of database name, charset and collate. The database
object structure is documented below.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Datastore</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#instancedatastore">Instance<wbr>Datastore</a></span>
    </dt>
    <dd>{{% md %}}An array of database engine type and version. The datastore
object structure is documented below. Changing this creates a new instance.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Flavor<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The flavor ID of the desired flavor for the instance.
Changing this creates new instance.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Database to be created on new instance. Changing this creates a
new instance.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Networks</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#instancenetwork">[]Instance<wbr>Network</a></span>
    </dt>
    <dd>{{% md %}}An array of one or more networks to attach to the
instance. The network object structure is documented below. Changing this
creates a new instance.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Region</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The region in which to create the db instance. Changing this
creates a new instance.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Size</span>
        <span class="property-indicator"></span>
        <span class="property-type">int</span>
    </dt>
    <dd>{{% md %}}Specifies the volume size in GB. Changing this creates new instance.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>Users</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#instanceuser">[]Instance<wbr>User</a></span>
    </dt>
    <dd>{{% md %}}An array of username, password, host and databases. The user
object structure is documented below.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-"
            title="">
        <span>configuration<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Configuration ID to be attached to the instance. Database instance
will be rebooted when configuration is detached.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>databases</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#instancedatabase">Instance<wbr>Database[]?</a></span>
    </dt>
    <dd>{{% md %}}An array of database name, charset and collate. The database
object structure is documented below.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>datastore</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#instancedatastore">Instance<wbr>Datastore</a></span>
    </dt>
    <dd>{{% md %}}An array of database engine type and version. The datastore
object structure is documented below. Changing this creates a new instance.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>flavor<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The flavor ID of the desired flavor for the instance.
Changing this creates new instance.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Database to be created on new instance. Changing this creates a
new instance.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>networks</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#instancenetwork">Instance<wbr>Network[]?</a></span>
    </dt>
    <dd>{{% md %}}An array of one or more networks to attach to the
instance. The network object structure is documented below. Changing this
creates a new instance.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>region</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}The region in which to create the db instance. Changing this
creates a new instance.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>size</span>
        <span class="property-indicator"></span>
        <span class="property-type">number</span>
    </dt>
    <dd>{{% md %}}Specifies the volume size in GB. Changing this creates new instance.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>users</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#instanceuser">Instance<wbr>User[]?</a></span>
    </dt>
    <dd>{{% md %}}An array of username, password, host and databases. The user
object structure is documented below.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-"
            title="">
        <span>configuration_<wbr>id</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Configuration ID to be attached to the instance. Database instance
will be rebooted when configuration is detached.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>databases</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#instancedatabase">List[Instance<wbr>Database]</a></span>
    </dt>
    <dd>{{% md %}}An array of database name, charset and collate. The database
object structure is documented below.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>datastore</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#instancedatastore">Dict[Instance<wbr>Datastore]</a></span>
    </dt>
    <dd>{{% md %}}An array of database engine type and version. The datastore
object structure is documented below. Changing this creates a new instance.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>flavor_<wbr>id</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The flavor ID of the desired flavor for the instance.
Changing this creates new instance.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Database to be created on new instance. Changing this creates a
new instance.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>networks</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#instancenetwork">List[Instance<wbr>Network]</a></span>
    </dt>
    <dd>{{% md %}}An array of one or more networks to attach to the
instance. The network object structure is documented below. Changing this
creates a new instance.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>region</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The region in which to create the db instance. Changing this
creates a new instance.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>size</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}Specifies the volume size in GB. Changing this creates new instance.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span>users</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#instanceuser">List[Instance<wbr>User]</a></span>
    </dt>
    <dd>{{% md %}}An array of username, password, host and databases. The user
object structure is documented below.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}








## Look up an Existing Instance Resource

Get an existing Instance resource's state with the given name, ID, and optional extra properties used to qualify the lookup.

{{< chooser language "javascript,typescript,python,go,csharp  " / >}}

{{% choosable language nodejs %}}
<div class="highlight"><pre class="chroma"><code class="language-typescript" data-lang="typescript"><span class="k">public static </span><span class="nf">get</span><span class="p">(</span><span class="nx">name</span>: <span class="nx"><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string">string</a></span><span class="p">, </span><span class="nx">id</span>: <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/pulumi/#ID">Input&lt;ID&gt;</a></span><span class="p">, </span><span class="nx">state</span>?: <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/openstack/database/#InstanceState">InstanceState</a></span><span class="p">, </span><span class="nx">opts</span>?: <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/pulumi/#CustomResourceOptions">CustomResourceOptions</a></span><span class="p">): </span><span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/openstack/database/#Instance">Instance</a></span></code></pre></div>
{{% /choosable %}}

{{% choosable language python %}}
<div class="highlight"><pre class="chroma"><code class="language-python" data-lang="python"><span class="k">static </span><span class="nf">get</span><span class="p">(resource_name, id, opts=None, </span>configuration_id=None<span class="p">, </span>databases=None<span class="p">, </span>datastore=None<span class="p">, </span>flavor_id=None<span class="p">, </span>name=None<span class="p">, </span>networks=None<span class="p">, </span>region=None<span class="p">, </span>size=None<span class="p">, </span>users=None<span class="p">, __props__=None);</span></code></pre></div>
{{% /choosable %}}

{{% choosable language go %}}
<div class="highlight"><pre class="chroma"><code class="language-go" data-lang="go"><span class="k">func </span>GetInstance<span class="p">(</span><span class="nx">ctx</span> *<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#Context">Context</a></span><span class="p">, </span><span class="nx">name</span> <span class="nx"><a href="https://golang.org/pkg/builtin/#string">string</a></span><span class="p">, </span><span class="nx">id</span> <span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#IDInput">IDInput</a></span><span class="p">, </span><span class="nx">state</span> *<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi-openstack/sdk/go/openstack/database?tab=doc#InstanceState">InstanceState</a></span><span class="p">, </span><span class="nx">opts</span> ...<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/go/pulumi?tab=doc#ResourceOption">ResourceOption</a></span><span class="p">) (*<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi-openstack/sdk/go/openstack/database?tab=doc#Instance">Instance</a></span>, error)</span></code></pre></div>
{{% /choosable %}}

{{% choosable language csharp %}}
<div class="highlight"><pre class="chroma"><code class="language-csharp" data-lang="csharp"><span class="k">public static </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi.Openstack/Pulumi.Openstack.Database.Instance.html">Instance</a></span><span class="nf"> Get</span><span class="p">(</span><span class="nx"><a href="https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/built-in-types">string</a></span> <span class="nx">name<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi/Pulumi.Input.html">Input&lt;string&gt;</a></span> <span class="nx">id<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi.Openstack/Pulumi.Openstack.Database.InstanceState.html">InstanceState</a></span>? <span class="nx">state<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi/Pulumi.CustomResourceOptions.html">CustomResourceOptions</a></span>? <span class="nx">opts = null<span class="p">)</span></code></pre></div>
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
        <span>Configuration<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Configuration ID to be attached to the instance. Database instance
will be rebooted when configuration is detached.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Databases</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#instancedatabase">List&lt;Instance<wbr>Database<wbr>Args&gt;?</a></span>
    </dt>
    <dd>{{% md %}}An array of database name, charset and collate. The database
object structure is documented below.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Datastore</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#instancedatastore">Instance<wbr>Datastore<wbr>Args?</a></span>
    </dt>
    <dd>{{% md %}}An array of database engine type and version. The datastore
object structure is documented below. Changing this creates a new instance.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Flavor<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}The flavor ID of the desired flavor for the instance.
Changing this creates new instance.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Database to be created on new instance. Changing this creates a
new instance.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Networks</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#instancenetwork">List&lt;Instance<wbr>Network<wbr>Args&gt;?</a></span>
    </dt>
    <dd>{{% md %}}An array of one or more networks to attach to the
instance. The network object structure is documented below. Changing this
creates a new instance.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Region</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}The region in which to create the db instance. Changing this
creates a new instance.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Size</span>
        <span class="property-indicator"></span>
        <span class="property-type">int?</span>
    </dt>
    <dd>{{% md %}}Specifies the volume size in GB. Changing this creates new instance.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Users</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#instanceuser">List&lt;Instance<wbr>User<wbr>Args&gt;?</a></span>
    </dt>
    <dd>{{% md %}}An array of username, password, host and databases. The user
object structure is documented below.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Configuration<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}Configuration ID to be attached to the instance. Database instance
will be rebooted when configuration is detached.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Databases</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#instancedatabase">[]Instance<wbr>Database</a></span>
    </dt>
    <dd>{{% md %}}An array of database name, charset and collate. The database
object structure is documented below.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Datastore</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#instancedatastore">*Instance<wbr>Datastore</a></span>
    </dt>
    <dd>{{% md %}}An array of database engine type and version. The datastore
object structure is documented below. Changing this creates a new instance.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Flavor<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}The flavor ID of the desired flavor for the instance.
Changing this creates new instance.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}Database to be created on new instance. Changing this creates a
new instance.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Networks</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#instancenetwork">[]Instance<wbr>Network</a></span>
    </dt>
    <dd>{{% md %}}An array of one or more networks to attach to the
instance. The network object structure is documented below. Changing this
creates a new instance.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Region</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}The region in which to create the db instance. Changing this
creates a new instance.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Size</span>
        <span class="property-indicator"></span>
        <span class="property-type">*int</span>
    </dt>
    <dd>{{% md %}}Specifies the volume size in GB. Changing this creates new instance.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Users</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#instanceuser">[]Instance<wbr>User</a></span>
    </dt>
    <dd>{{% md %}}An array of username, password, host and databases. The user
object structure is documented below.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>configuration<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Configuration ID to be attached to the instance. Database instance
will be rebooted when configuration is detached.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>databases</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#instancedatabase">Instance<wbr>Database[]?</a></span>
    </dt>
    <dd>{{% md %}}An array of database name, charset and collate. The database
object structure is documented below.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>datastore</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#instancedatastore">Instance<wbr>Datastore?</a></span>
    </dt>
    <dd>{{% md %}}An array of database engine type and version. The datastore
object structure is documented below. Changing this creates a new instance.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>flavor<wbr>Id</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}The flavor ID of the desired flavor for the instance.
Changing this creates new instance.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Database to be created on new instance. Changing this creates a
new instance.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>networks</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#instancenetwork">Instance<wbr>Network[]?</a></span>
    </dt>
    <dd>{{% md %}}An array of one or more networks to attach to the
instance. The network object structure is documented below. Changing this
creates a new instance.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>region</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}The region in which to create the db instance. Changing this
creates a new instance.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>size</span>
        <span class="property-indicator"></span>
        <span class="property-type">number?</span>
    </dt>
    <dd>{{% md %}}Specifies the volume size in GB. Changing this creates new instance.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>users</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#instanceuser">Instance<wbr>User[]?</a></span>
    </dt>
    <dd>{{% md %}}An array of username, password, host and databases. The user
object structure is documented below.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>configuration_<wbr>id</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Configuration ID to be attached to the instance. Database instance
will be rebooted when configuration is detached.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>databases</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#instancedatabase">List[Instance<wbr>Database]</a></span>
    </dt>
    <dd>{{% md %}}An array of database name, charset and collate. The database
object structure is documented below.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>datastore</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#instancedatastore">Dict[Instance<wbr>Datastore]</a></span>
    </dt>
    <dd>{{% md %}}An array of database engine type and version. The datastore
object structure is documented below. Changing this creates a new instance.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>flavor_<wbr>id</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The flavor ID of the desired flavor for the instance.
Changing this creates new instance.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Database to be created on new instance. Changing this creates a
new instance.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>networks</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#instancenetwork">List[Instance<wbr>Network]</a></span>
    </dt>
    <dd>{{% md %}}An array of one or more networks to attach to the
instance. The network object structure is documented below. Changing this
creates a new instance.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>region</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The region in which to create the db instance. Changing this
creates a new instance.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>size</span>
        <span class="property-indicator"></span>
        <span class="property-type">float</span>
    </dt>
    <dd>{{% md %}}Specifies the volume size in GB. Changing this creates new instance.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>users</span>
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#instanceuser">List[Instance<wbr>User]</a></span>
    </dt>
    <dd>{{% md %}}An array of username, password, host and databases. The user
object structure is documented below.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}










## Supporting Types

<h4>Instance<wbr>Database</h4>
{{% choosable language nodejs %}}
> See the <a href="/docs/reference/pkg/nodejs/pulumi/openstack/types/input/#InstanceDatabase">input</a> and <a href="/docs/reference/pkg/nodejs/pulumi/openstack/types/output/#InstanceDatabase">output</a> API doc for this type.
{{% /choosable %}}

{{% choosable language go %}}
> See the <a href="https://pkg.go.dev/github.com/pulumi/pulumi-openstack/sdk/go/openstack/database?tab=doc#InstanceDatabaseArgs">input</a> and <a href="https://pkg.go.dev/github.com/pulumi/pulumi-openstack/sdk/go/openstack/database?tab=doc#InstanceDatabaseOutput">output</a> API doc for this type.
{{% /choosable %}}




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Charset</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Database character set. Changing this creates a
new instance.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Collate</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Database collation. Changing this creates a new instance.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Database to be created on new instance. Changing this creates a
new instance.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Charset</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}Database character set. Changing this creates a
new instance.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Collate</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}Database collation. Changing this creates a new instance.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Database to be created on new instance. Changing this creates a
new instance.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>charset</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Database character set. Changing this creates a
new instance.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>collate</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Database collation. Changing this creates a new instance.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Database to be created on new instance. Changing this creates a
new instance.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>charset</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Database character set. Changing this creates a
new instance.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>collate</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Database collation. Changing this creates a new instance.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Database to be created on new instance. Changing this creates a
new instance.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}





<h4>Instance<wbr>Datastore</h4>
{{% choosable language nodejs %}}
> See the <a href="/docs/reference/pkg/nodejs/pulumi/openstack/types/input/#InstanceDatastore">input</a> and <a href="/docs/reference/pkg/nodejs/pulumi/openstack/types/output/#InstanceDatastore">output</a> API doc for this type.
{{% /choosable %}}

{{% choosable language go %}}
> See the <a href="https://pkg.go.dev/github.com/pulumi/pulumi-openstack/sdk/go/openstack/database?tab=doc#InstanceDatastoreArgs">input</a> and <a href="https://pkg.go.dev/github.com/pulumi/pulumi-openstack/sdk/go/openstack/database?tab=doc#InstanceDatastoreOutput">output</a> API doc for this type.
{{% /choosable %}}




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>Type</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Database engine type to be used in new instance. Changing this
creates a new instance.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Version</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Version of database engine type to be used in new instance.
Changing this creates a new instance.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>Type</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Database engine type to be used in new instance. Changing this
creates a new instance.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Version</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Version of database engine type to be used in new instance.
Changing this creates a new instance.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>type</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Database engine type to be used in new instance. Changing this
creates a new instance.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>version</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Version of database engine type to be used in new instance.
Changing this creates a new instance.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span>type</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Database engine type to be used in new instance. Changing this
creates a new instance.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>version</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Version of database engine type to be used in new instance.
Changing this creates a new instance.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}





<h4>Instance<wbr>Network</h4>
{{% choosable language nodejs %}}
> See the <a href="/docs/reference/pkg/nodejs/pulumi/openstack/types/input/#InstanceNetwork">input</a> and <a href="/docs/reference/pkg/nodejs/pulumi/openstack/types/output/#InstanceNetwork">output</a> API doc for this type.
{{% /choosable %}}

{{% choosable language go %}}
> See the <a href="https://pkg.go.dev/github.com/pulumi/pulumi-openstack/sdk/go/openstack/database?tab=doc#InstanceNetworkArgs">input</a> and <a href="https://pkg.go.dev/github.com/pulumi/pulumi-openstack/sdk/go/openstack/database?tab=doc#InstanceNetworkOutput">output</a> API doc for this type.
{{% /choosable %}}




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Fixed<wbr>Ip<wbr>V4</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Specifies a fixed IPv4 address to be used on this
network. Changing this creates a new instance.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Fixed<wbr>Ip<wbr>V6</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Specifies a fixed IPv6 address to be used on this
network. Changing this creates a new instance.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Port</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}The port UUID of a
network to attach to the instance. Changing this creates a new instance.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Uuid</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}The network UUID to
attach to the instance. Changing this creates a new instance.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Fixed<wbr>Ip<wbr>V4</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}Specifies a fixed IPv4 address to be used on this
network. Changing this creates a new instance.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Fixed<wbr>Ip<wbr>V6</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}Specifies a fixed IPv6 address to be used on this
network. Changing this creates a new instance.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Port</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}The port UUID of a
network to attach to the instance. Changing this creates a new instance.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Uuid</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}The network UUID to
attach to the instance. Changing this creates a new instance.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>fixed<wbr>Ip<wbr>V4</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Specifies a fixed IPv4 address to be used on this
network. Changing this creates a new instance.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>fixed<wbr>Ip<wbr>V6</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}Specifies a fixed IPv6 address to be used on this
network. Changing this creates a new instance.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>port</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}The port UUID of a
network to attach to the instance. Changing this creates a new instance.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>uuid</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}The network UUID to
attach to the instance. Changing this creates a new instance.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>fixed<wbr>Ip<wbr>V4</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Specifies a fixed IPv4 address to be used on this
network. Changing this creates a new instance.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>fixed<wbr>Ip<wbr>V6</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Specifies a fixed IPv6 address to be used on this
network. Changing this creates a new instance.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>port</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The port UUID of a
network to attach to the instance. Changing this creates a new instance.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>uuid</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}The network UUID to
attach to the instance. Changing this creates a new instance.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}





<h4>Instance<wbr>User</h4>
{{% choosable language nodejs %}}
> See the <a href="/docs/reference/pkg/nodejs/pulumi/openstack/types/input/#InstanceUser">input</a> and <a href="/docs/reference/pkg/nodejs/pulumi/openstack/types/output/#InstanceUser">output</a> API doc for this type.
{{% /choosable %}}

{{% choosable language go %}}
> See the <a href="https://pkg.go.dev/github.com/pulumi/pulumi-openstack/sdk/go/openstack/database?tab=doc#InstanceUserArgs">input</a> and <a href="https://pkg.go.dev/github.com/pulumi/pulumi-openstack/sdk/go/openstack/database?tab=doc#InstanceUserOutput">output</a> API doc for this type.
{{% /choosable %}}




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Databases</span>
        <span class="property-indicator"></span>
        <span class="property-type">List<string>?</span>
    </dt>
    <dd>{{% md %}}A list of databases that user will have access to. If not specified, 
user has access to all databases on th einstance. Changing this creates a new instance.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Host</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}An ip address or % sign indicating what ip addresses can connect with
this user credentials. Changing this creates a new instance.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Database to be created on new instance. Changing this creates a
new instance.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Password</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}User's password. Changing this creates a
new instance.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>Databases</span>
        <span class="property-indicator"></span>
        <span class="property-type">[]string</span>
    </dt>
    <dd>{{% md %}}A list of databases that user will have access to. If not specified, 
user has access to all databases on th einstance. Changing this creates a new instance.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Host</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}An ip address or % sign indicating what ip addresses can connect with
this user credentials. Changing this creates a new instance.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>Name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Database to be created on new instance. Changing this creates a
new instance.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>Password</span>
        <span class="property-indicator"></span>
        <span class="property-type">*string</span>
    </dt>
    <dd>{{% md %}}User's password. Changing this creates a
new instance.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>databases</span>
        <span class="property-indicator"></span>
        <span class="property-type">string[]?</span>
    </dt>
    <dd>{{% md %}}A list of databases that user will have access to. If not specified, 
user has access to all databases on th einstance. Changing this creates a new instance.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>host</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}An ip address or % sign indicating what ip addresses can connect with
this user credentials. Changing this creates a new instance.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">string</span>
    </dt>
    <dd>{{% md %}}Database to be created on new instance. Changing this creates a
new instance.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>password</span>
        <span class="property-indicator"></span>
        <span class="property-type">string?</span>
    </dt>
    <dd>{{% md %}}User's password. Changing this creates a
new instance.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-optional"
            title="Optional">
        <span>databases</span>
        <span class="property-indicator"></span>
        <span class="property-type">List[str]</span>
    </dt>
    <dd>{{% md %}}A list of databases that user will have access to. If not specified, 
user has access to all databases on th einstance. Changing this creates a new instance.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>host</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}An ip address or % sign indicating what ip addresses can connect with
this user credentials. Changing this creates a new instance.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span>name</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}Database to be created on new instance. Changing this creates a
new instance.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span>password</span>
        <span class="property-indicator"></span>
        <span class="property-type">str</span>
    </dt>
    <dd>{{% md %}}User's password. Changing this creates a
new instance.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}









<h3>Package Details</h3>
<dl class="package-details">
	<dt>Repository</dt>
	<dd><a href="https://github.com/pulumi/pulumi-openstack">https://github.com/pulumi/pulumi-openstack</a></dd>
	<dt>License</dt>
	<dd>Apache-2.0</dd>
    
</dl>
