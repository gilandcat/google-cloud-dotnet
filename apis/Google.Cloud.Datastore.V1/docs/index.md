# Google.Cloud.Datastore.V1

`Google.Cloud.Datastore.V1` is a .NET client library for [Google
Cloud Datastore](https://cloud.google.com/datastore/docs/concepts/overview).

# Installation

Install the `Google.Cloud.Datastore.V1` package from NuGet. Add it to
your project in the normal way (for example by right-clicking on the
project in Visual Studio and choosing "Manage NuGet Packages...").

# Authentication

To authenticate all your API calls, first install and setup the
[Google Cloud SDK](https://cloud.google.com/sdk/). After that is
installed, run the following command in a Google Cloud SDK Shell:

```sh
> gcloud auth application-default login
```

# Getting started

See the [Datastore Quickstart](https://cloud.google.com/datastore/docs/quickstart) for an introduction with runnable code samples.

The [DatastoreDb](obj/api/Google.Cloud.Datastore.V1.DatastoreDb.yml)
class is provided as a wrapper for
[DatastoreClient](obj/api/Google.Cloud.Datastore.V1.DatastoreClient.yml),
simplifying operations considerably by assuming all operations act
on the same partition, and providing page streaming operations on
structured query results.

Several custom conversions, additional constructors,
factory methods (particularly on [Filter](obj/api/Google.Cloud.Datastore.V1.Filter.yml)
are provided to simplify working with the protobuf messages.

# Sample code

Inserting data:

[!code-cs[](obj/snippets/Google.Cloud.Datastore.V1.DatastoreDb.txt#InsertOverview)]

Querying data:

[!code-cs[](obj/snippets/Google.Cloud.Datastore.V1.DatastoreDb.txt#QueryOverview)]

Lots more samples:
[github.com/GoogleCloudPlatform/dotnet-docs-samples](https://github.com/GoogleCloudPlatform/dotnet-docs-samples/tree/master/datastore/api)
