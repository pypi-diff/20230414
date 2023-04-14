# Comparing `tmp/copernicus_marine_client-0.4.0.tar.gz` & `tmp/copernicus_marine_client-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "copernicus_marine_client-0.4.0.tar", max compression
+gzip compressed data, was "copernicus_marine_client-0.5.0.tar", max compression
```

## Comparing `copernicus_marine_client-0.4.0.tar` & `copernicus_marine_client-0.5.0.tar`

### file list

```diff
@@ -1,14 +1,16 @@
--rw-r--r--   0        0        0       13 2023-02-28 10:55:38.192830 copernicus_marine_client-0.4.0/copernicus_marine_client/__init__.py
--rw-r--r--   0        0        0       13 2023-02-28 10:55:38.193838 copernicus_marine_client-0.4.0/copernicus_marine_client/catalogue_parser/__init__.py
--rw-r--r--   0        0        0    11437 2023-04-05 12:12:52.792317 copernicus_marine_client-0.4.0/copernicus_marine_client/catalogue_parser/catalogue_parser.py
--rw-r--r--   0        0        0       13 2023-03-27 15:21:46.450744 copernicus_marine_client-0.4.0/copernicus_marine_client/command_line_interface/__init__.py
--rw-r--r--   0        0        0      514 2023-04-04 08:48:14.516284 copernicus_marine_client-0.4.0/copernicus_marine_client/command_line_interface/copernicus_marine.py
--rw-r--r--   0        0        0     4434 2023-04-04 08:48:14.517234 copernicus_marine_client-0.4.0/copernicus_marine_client/command_line_interface/group_describe.py
--rw-r--r--   0        0        0     6197 2023-04-05 12:12:52.805382 copernicus_marine_client-0.4.0/copernicus_marine_client/command_line_interface/group_native.py
--rw-r--r--   0        0        0     9822 2023-04-05 12:12:52.807381 copernicus_marine_client-0.4.0/copernicus_marine_client/command_line_interface/group_subset.py
--rw-r--r--   0        0        0     6915 2023-04-04 08:48:14.525199 copernicus_marine_client-0.4.0/copernicus_marine_client/download_functions/download_ftp.py
--rw-r--r--   0        0        0     2595 2023-04-05 12:12:52.809382 copernicus_marine_client-0.4.0/copernicus_marine_client/download_functions/download_motu.py
--rw-r--r--   0        0        0      755 2023-04-05 12:13:30.724782 copernicus_marine_client-0.4.0/pyproject.toml
--rw-r--r--   0        0        0    11034 2023-04-05 12:12:52.789314 copernicus_marine_client-0.4.0/README.md
--rw-r--r--   0        0        0    12172 1970-01-01 00:00:00.000000 copernicus_marine_client-0.4.0/setup.py
--rw-r--r--   0        0        0    11424 1970-01-01 00:00:00.000000 copernicus_marine_client-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0       13 2023-02-28 10:55:38.192830 copernicus_marine_client-0.5.0/copernicus_marine_client/__init__.py
+-rw-r--r--   0        0        0       13 2023-02-28 10:55:38.193838 copernicus_marine_client-0.5.0/copernicus_marine_client/catalogue_parser/__init__.py
+-rw-r--r--   0        0        0    10868 2023-04-14 09:01:19.325083 copernicus_marine_client-0.5.0/copernicus_marine_client/catalogue_parser/catalogue_parser.py
+-rw-r--r--   0        0        0     3978 2023-04-14 09:01:19.328098 copernicus_marine_client-0.5.0/copernicus_marine_client/catalogue_parser/request_structure.py
+-rw-r--r--   0        0        0       13 2023-03-27 15:21:46.450744 copernicus_marine_client-0.5.0/copernicus_marine_client/command_line_interface/__init__.py
+-rw-r--r--   0        0        0      514 2023-04-04 08:48:14.516284 copernicus_marine_client-0.5.0/copernicus_marine_client/command_line_interface/copernicus_marine.py
+-rw-r--r--   0        0        0     3282 2023-04-14 06:39:18.368218 copernicus_marine_client-0.5.0/copernicus_marine_client/command_line_interface/group_describe.py
+-rw-r--r--   0        0        0     4874 2023-04-14 09:01:19.330085 copernicus_marine_client-0.5.0/copernicus_marine_client/command_line_interface/group_native.py
+-rw-r--r--   0        0        0     9147 2023-04-14 09:02:50.587339 copernicus_marine_client-0.5.0/copernicus_marine_client/command_line_interface/group_subset.py
+-rw-r--r--   0        0        0     7548 2023-04-14 09:01:19.334097 copernicus_marine_client-0.5.0/copernicus_marine_client/download_functions/download_ftp.py
+-rw-r--r--   0        0        0     3780 2023-04-14 09:01:19.336102 copernicus_marine_client-0.5.0/copernicus_marine_client/download_functions/download_motu.py
+-rw-r--r--   0        0        0     1037 2023-04-14 09:01:19.337099 copernicus_marine_client-0.5.0/copernicus_marine_client/download_functions/download_opendap.py
+-rw-r--r--   0        0        0      755 2023-04-14 09:00:51.005137 copernicus_marine_client-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0    11857 2023-04-14 09:01:19.321085 copernicus_marine_client-0.5.0/README.md
+-rw-r--r--   0        0        0    12988 1970-01-01 00:00:00.000000 copernicus_marine_client-0.5.0/setup.py
+-rw-r--r--   0        0        0    12251 1970-01-01 00:00:00.000000 copernicus_marine_client-0.5.0/PKG-INFO
```

### Comparing `copernicus_marine_client-0.4.0/copernicus_marine_client/command_line_interface/copernicus_marine.py` & `copernicus_marine_client-0.5.0/copernicus_marine_client/command_line_interface/copernicus_marine.py`

 * *Files identical despite different names*

### Comparing `copernicus_marine_client-0.4.0/copernicus_marine_client/command_line_interface/group_describe.py` & `copernicus_marine_client-0.5.0/copernicus_marine_client/command_line_interface/group_describe.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,68 +1,44 @@
-import warnings
 from json import dumps
+from typing import Any
 
 import click
 
 from copernicus_marine_client.catalogue_parser.catalogue_parser import (
     CopernicusMarineCatalogue,
     filter_catalogue_with_strings,
     parse_catalogue,
 )
 
-warnings.filterwarnings(
-    "ignore",
-    message="the .identification and"
-    + " .serviceidentification properties will merge into .identification"
-    + " being a list of properties.  This is currently implemented in"
-    + " .identificationinfo.  "
-    + "Please see https://github.com/geopython/OWSLib/issues/38 for more "
-    + "information",
-)
-warnings.filterwarnings(
-    "ignore",
-    message="The .keywords and .keywords2 properties will merge into the"
-    + " .keywords property in the future, with .keywords becoming a list of"
-    + " MD_Keywords instances. This is currently implemented in .keywords2."
-    + " Please see https://github.com/geopython/OWSLib/issues/301 for more "
-    + "information",
-)
-warnings.filterwarnings(
-    "ignore",
-    message="The .keywords_object attribute will become .keywords proper in "
-    + "the next release. .keywords_object is a list of ibstances of the "
-    + "Keyword class. See for https://github.com/geopython/OWSLib/pull/765"
-    + " more details.",
-)
-
 
 @click.group()
 def cli_group_describe() -> None:
     pass
 
 
 @cli_group_describe.command(
     "describe",
-    help="""Parse the Copernicus Marine catalogue, then display a
-        JSON-ified version of the corresponding python object.
+    help="""
+    Parse the Copernicus Marine catalogue, then display a
+    JSON-ified version of the corresponding python object.
 
-        The default display contains information on the products, and more data
-        can be displayed using the _include-<argument>_ flags (see Usage section).
+    The default display contains information on the products, and more data
+    can be displayed using the _include-<argument>_ flags (see Usage section).
 
-        The _contains_ option allows the user to specify one or several strings to
-        filter through the catalogue display. The search is performed recursively
-        on all attributes of the catalogue, and the tokens only need to be
-        contained in one of the attributes (i.e. not exact match).
+    The _contains_ option allows the user to specify one or several strings to
+    filter through the catalogue display. The search is performed recursively
+    on all attributes of the catalogue, and the tokens only need to be
+    contained in one of the attributes (i.e. not exact match).
 
-        Example:
+    Example:
 
-        > copernicus-marine describe --contains METOFFICE-GLO-SST-L4-NRT-OBS-SST-V2
-        --include-datasets
+    > copernicus-marine describe --contains METOFFICE-GLO-SST-L4-NRT-OBS-SST-V2
+    --include-datasets
 
-        > copernicus-marine describe -c METOFFICE-GLO-SST-L4-NRT-OBS-SST-V2
+    > copernicus-marine describe -c METOFFICE-GLO-SST-L4-NRT-OBS-SST-V2
         """,
 )
 @click.option(
     "--one-line",
     type=bool,
     is_flag=True,
     default=False,
@@ -79,21 +55,14 @@
     "--include-datasets",
     type=bool,
     is_flag=True,
     default=False,
     help="Include product dataset details in output",
 )
 @click.option(
-    "--include-providers",
-    type=bool,
-    is_flag=True,
-    default=False,
-    help="Include product provider details in output",
-)
-@click.option(
     "--include-keywords",
     type=bool,
     is_flag=True,
     default=False,
     help="Include product keyword details in output",
 )
 @click.option(
@@ -110,41 +79,44 @@
     is_flag=True,
     default=False,
     help="Force to refresh the catalogue by overwriting the local cache",
 )
 def describe(
     include_description: bool,
     include_datasets: bool,
-    include_providers: bool,
     include_keywords: bool,
     one_line: bool,
     contains: list[str],
     overwrite_cache: bool,
 ) -> None:
-    catalogue: CopernicusMarineCatalogue = parse_catalogue(
+    base_catalogue: CopernicusMarineCatalogue = parse_catalogue(
         overwrite_cache=overwrite_cache
     )
+    catalogue: Any
     if contains:
-        catalogue = filter_catalogue_with_strings(catalogue, contains)
+        filtered_catalogue = filter_catalogue_with_strings(
+            base_catalogue, contains
+        )
+        catalogue = filtered_catalogue or {}
+    else:
+        catalogue = base_catalogue
 
     def default_filter(obj):
         attributes = obj.__dict__
         if not include_description:
             attributes.pop("description", None)
         if not include_datasets:
             attributes.pop("datasets", None)
-        if not include_providers:
-            attributes.pop("providers", None)
         if not include_keywords:
             attributes.pop("keywords", None)
         return obj.__dict__
 
     json_dump = (
-        dumps(catalogue, default=default_filter)
+        dumps(catalogue, default=default_filter, sort_keys=True)
         if one_line
-        else dumps(catalogue, default=default_filter, indent=2)
+        else dumps(catalogue, default=default_filter, sort_keys=True, indent=2)
     )
     click.echo(json_dump)
 
 
 if __name__ == "__main__":
     cli_group_describe()
```

### Comparing `copernicus_marine_client-0.4.0/copernicus_marine_client/command_line_interface/group_subset.py` & `copernicus_marine_client-0.5.0/copernicus_marine_client/command_line_interface/group_subset.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,100 +1,67 @@
 from datetime import datetime
-from typing import List, Optional, Tuple
+from typing import List, Optional
 
 import click
-from opendap_downloader.opendap_downloader import (
-    download_dataset as download_opendap,
-)
 
 from copernicus_marine_client.catalogue_parser.catalogue_parser import (
     MOTU_KEY,
     OPENDAP_KEY,
     get_dataset_url_from_id,
     get_protocol_from_url,
     parse_catalogue,
 )
+from copernicus_marine_client.catalogue_parser.request_structure import (
+    SubsetRequest,
+    subset_request_from_file,
+)
 from copernicus_marine_client.download_functions.download_motu import (
     download_motu,
 )
+from copernicus_marine_client.download_functions.download_opendap import (
+    download_opendap,
+)
 
-PROTOCOL_KEYS_ORDER = [OPENDAP_KEY]
-
-
-class Mutex(click.Option):
-    def __init__(self, *args, **kwargs):
-        self.not_required_if: list = kwargs.pop("not_required_if")
-
-        assert self.not_required_if, "'not_required_if' parameter required"
-        kwargs["help"] = (
-            kwargs.get("help", "")
-            + " option is mutually exclusive with "
-            + ", ".join(self.not_required_if)
-            + "."
-        ).strip()
-        super().__init__(*args, **kwargs)
-
-    def handle_parse_result(self, ctx, opts, args):
-        current_opt: bool = self.name in opts
-        for mutex_opt in self.not_required_if:
-            if mutex_opt in opts:
-                if current_opt:
-                    raise click.UsageError(
-                        "Illegal usage: '"
-                        + str(self.name)
-                        + "' is mutually exclusive with "
-                        + str(mutex_opt)
-                        + "."
-                    )
-                else:
-                    self.prompt = None
-        return super().handle_parse_result(ctx, opts, args)
+PROTOCOL_KEYS_ORDER = {"opendap": OPENDAP_KEY, "motu": MOTU_KEY}
 
 
 @click.group()
 def cli_group_subset() -> None:
     pass
 
 
 @cli_group_subset.command(
     "subset",
-    help="""Downloads subsets of datasets as NetCDF files taking into account the
-server data query limit. A 'dataset-id' (can be found via the
-'copernicus-marine describe' command) is required.
+    help="""Downloads subsets of datasets as NetCDF files.
+    Either one of 'dataset-id' or 'dataset-url' is required
+    (can be found via the 'copernicus-marine describe' command).
 
 Example:
 
   copernicus-marine subset
 --dataset-id METOFFICE-GLO-SST-L4-NRT-OBS-SST-V2
 --variable analysed_sst --variable sea_ice_fraction
---temporal-subset 2021-01-01 2021-01-02
---geographical-subset 0.0 0.1 0.0 0.1
+--start-datetime 2021-01-01 --end-datetime 2021-01-02
+--minimal-longitude 0.0 --maximal-longitude 0.1
+--minimal-latitude 0.0 --maximal-latitude 0.1
 
   copernicus-marine subset -i METOFFICE-GLO-SST-L4-NRT-OBS-SST-V2 -v analysed_sst
-  -v sea_ice_fraction -t 2021-01-01 2021-01-02 -g 0.0 0.1 0.0 0.1
+  -v sea_ice_fraction -t 2021-01-01 -T 2021-01-02 -x 0.0 -X 0.1 -y 0.0 -Y 0.1
 """,
 )
 @click.option(
     "--dataset-url",
     "-u",
     type=str,
-    cls=Mutex,
-    not_required_if=[
-        "dataset_id",
-    ],
     help="The full dataset URL",
 )
 @click.option(
     "--dataset-id",
     "-i",
     type=str,
-    cls=Mutex,
-    not_required_if=[
-        "dataset_url",
-    ],
     help="The dataset id",
 )
 @click.option(
     "--login",
     prompt=True,
     hide_input=False,
 )
@@ -108,236 +75,242 @@
     "-v",
     "variables",
     type=str,
     help="Specify dataset variables",
     multiple=True,
 )
 @click.option(
-    "--geographical-subset",
-    "-g",
-    type=(
-        click.FloatRange(min=-90, max=90),
-        click.FloatRange(min=-90, max=90),
-        click.FloatRange(min=-180, max=180),
-        click.FloatRange(min=-180, max=180),
-    ),
-    help="The geographical subset as "
-    + "minimal latitude, maximal latitude, "
-    + "minimal longitude and maximal longitude",
+    "--minimal-longitude",
+    "-x",
+    type=click.FloatRange(min=-180, max=180),
+    help="Minimal longitude for the subset",
+)
+@click.option(
+    "--maximal-longitude",
+    "-X",
+    type=click.FloatRange(min=-180, max=180),
+    help="Maximal longitude for the subset",
+)
+@click.option(
+    "--minimal-latitude",
+    "-y",
+    type=click.FloatRange(min=-90, max=90),
+    help="Minimal latitude for the subset",
+)
+@click.option(
+    "--maximal-latitude",
+    "-Y",
+    type=click.FloatRange(min=-90, max=90),
+    help="Maximal latitude for the subset",
+)
+@click.option(
+    "--minimal-depth",
+    "-z",
+    type=click.FloatRange(min=0),
+    help="Minimal depth for the subset",
 )
 @click.option(
-    "--temporal-subset",
+    "--maximal-depth",
+    "-Z",
+    type=click.FloatRange(min=0),
+    help="Maximal depth for the subset",
+)
+@click.option(
+    "--start-datetime",
     "-t",
-    type=(
-        click.DateTime(
-            ["%Y", "%Y-%m-%d", "%Y-%m-%dT%H:%M:%S", "%Y-%m-%d %H:%M:%S"]
-        ),
-        click.DateTime(
-            ["%Y", "%Y-%m-%d", "%Y-%m-%dT%H:%M:%S", "%Y-%m-%d %H:%M:%S"]
-        ),
+    type=click.DateTime(
+        ["%Y", "%Y-%m-%d", "%Y-%m-%dT%H:%M:%S", "%Y-%m-%d %H:%M:%S"]
     ),
-    help="The temporal subset as start datetime and end datetime",
+    help="The start datetime of the temporal subset",
 )
 @click.option(
-    "--depth-range",
-    "-d",
-    type=(click.FloatRange(min=0), click.FloatRange(min=0)),
-    help="The depth range in meters, if depth is a dataset coordinate",
+    "--end-datetime",
+    "-T",
+    type=click.DateTime(
+        ["%Y", "%Y-%m-%d", "%Y-%m-%dT%H:%M:%S", "%Y-%m-%d %H:%M:%S"]
+    ),
+    help="The end datetime of the temporal subset",
 )
 @click.option(
-    "--output-path",
+    "--output-directory",
     "-o",
     type=click.Path(),
     required=True,
-    help="The destination path for the downloaded files."
+    help="The destination folder for the downloaded files."
     + " Default is the current directory",
     default="",
 )
 @click.option(
-    "--output-file",
+    "--output-filename",
     "-f",
     type=click.Path(),
     help="Concatenate the downloaded data in the given file name"
     + " (under the output path)",
 )
 @click.option(
-    "--limit",
-    "-l",
-    type=int,
-    help="Specify the download size limit (in MB) of the Opendap server if it "
-    "can't be provided by the message error",
-)
-@click.option(
-    "--confirmation",
+    "--assume-yes",
     is_flag=True,
-    help="Print dataset metadata and ask for confirmation before download",
+    help="Flag to skip confirmation before download",
 )
 @click.option(
     "--force-protocol",
-    type=click.Choice([OPENDAP_KEY, MOTU_KEY]),
+    type=click.Choice(list(PROTOCOL_KEYS_ORDER.keys())),
     help="Force download through one of the available protocols",
 )
 @click.option(
     "--dry-run",
     is_flag=True,
     default=False,
     help="Flag to specify NOT to send the request to external server. "
     "Returns the request instead",
 )
+@click.option(
+    "--request-file",
+    type=click.Path(),
+    help="Option to pass a filename corresponding to a file containg CLI arguments. "
+    "The file MUST follow the structure of dataclass 'SubsetRequest'. "
+    "ANY PARAMETER SPECIFIED ASIDE FROM FILE WILL NOT "
+    "BE TAKEN INTO CONSIDERATION FOR THE REQUEST IF FILE "
+    "IS SPECIFIED.",
+)
 def subset(
     dataset_url: str,
     dataset_id: str,
     login: str,
     password: str,
-    variables: List[str],
-    geographical_subset: Tuple[float, float, float, float],
-    temporal_subset: Tuple[datetime, datetime],
-    depth_range: Tuple[float, float],
-    output_path: str,
-    confirmation: bool,
-    output_file: Optional[str],
-    limit: Optional[int] = None,
-    force_protocol: Optional[str] = None,
-    dry_run: Optional[bool] = False,
+    variables: Optional[List[str]],
+    minimal_longitude: Optional[float],
+    maximal_longitude: Optional[float],
+    minimal_latitude: Optional[float],
+    maximal_latitude: Optional[float],
+    minimal_depth: Optional[float],
+    maximal_depth: Optional[float],
+    start_datetime: Optional[datetime],
+    end_datetime: Optional[datetime],
+    output_filename: Optional[str],
+    force_protocol: Optional[str],
+    request_file: Optional[str],
+    output_directory: str = "",
+    assume_yes: bool = False,
+    dry_run: bool = False,
 ):
+    if request_file:
+        subset_request = subset_request_from_file(request_file)
+    else:
+        subset_request = SubsetRequest(
+            dataset_url=dataset_url,
+            dataset_id=dataset_id,
+            variables=variables,
+            minimal_longitude=minimal_longitude,
+            maximal_longitude=maximal_longitude,
+            minimal_latitude=minimal_latitude,
+            maximal_latitude=maximal_latitude,
+            minimal_depth=minimal_depth,
+            maximal_depth=maximal_depth,
+            start_datetime=start_datetime,
+            end_datetime=end_datetime,
+            output_directory=output_directory,
+            output_filename=output_filename,
+            assume_yes=assume_yes,
+            force_protocol=force_protocol,
+            dry_run=dry_run,
+        )
     subset_function(
-        dataset_url,
-        dataset_id,
         login,
         password,
-        variables,
-        geographical_subset,
-        temporal_subset,
-        depth_range,
-        output_path,
-        confirmation,
-        output_file,
-        limit,
-        force_protocol,
-        dry_run,
+        subset_request,
     )
 
 
 def subset_function(
-    dataset_url: str,
-    dataset_id: str,
     login: str,
     password: str,
-    variables: List[str],
-    geographical_subset: Tuple[float, float, float, float],
-    temporal_subset: Tuple[datetime, datetime],
-    depth_range: Tuple[float, float],
-    output_path: str,
-    confirmation: bool,
-    output_file: Optional[str],
-    limit: Optional[int] = None,
-    force_protocol: Optional[str] = None,
-    dry_run: Optional[bool] = False,
+    subset_request: SubsetRequest,
 ):
     possible_protocols = (
-        PROTOCOL_KEYS_ORDER if not force_protocol else [force_protocol]
+        PROTOCOL_KEYS_ORDER.values()
+        if not subset_request.force_protocol
+        else [PROTOCOL_KEYS_ORDER[subset_request.force_protocol]]
     )
-    if force_protocol:
-        click.echo(f"You forced selection of protocol: {force_protocol}")
-    if not dataset_url:
-        if not dataset_id:
+    if subset_request.force_protocol:
+        click.echo(
+            f"You forced selection of protocol: {subset_request.force_protocol}"
+        )
+    if not subset_request.dataset_url:
+        if not subset_request.dataset_id:
             raise SyntaxError(
                 "Must specify at least one of 'dataset_url' or 'dataset_id'"
             )
         catalogue = parse_catalogue()
         protocol_keys_iterator = iter(possible_protocols)
-        while not dataset_url:
+        while not subset_request.dataset_url:
             try:
                 protocol = next(protocol_keys_iterator)
             except StopIteration:
                 raise KeyError(
-                    f"Dataset {dataset_id} does not have a valid protocol "
+                    f"Dataset {subset_request.dataset_id} does "
+                    "not have a valid protocol "
                     f"for subset function. Available protocols: {possible_protocols}"
                 )
-            dataset_url = get_dataset_url_from_id(
-                catalogue, dataset_id, protocol
+            subset_request.dataset_url = get_dataset_url_from_id(
+                catalogue, subset_request.dataset_id, protocol
             )
     else:
-        protocol = get_protocol_from_url(dataset_url)
+        protocol = get_protocol_from_url(subset_request.dataset_url)
         catalogue = None
-    if protocol == OPENDAP_KEY:
+    if (
+        subset_request.force_protocol
+        and protocol != subset_request.force_protocol
+    ):
+        raise AttributeError("Dataset url does not match forced protocol!")
+    elif protocol == OPENDAP_KEY:
         click.echo("download through OPeNDAP")
-        if dry_run:
+        if subset_request.dry_run:
             print(
                 "download_opendap("
                 + ", ".join(
                     [
                         f"{login}",
                         "HIDING_PASSWORD",
-                        f"{dataset_url}",
-                        f"{output_path}",
-                        f"{output_file}",
-                        f"{variables}",
-                        f"{geographical_subset}",
-                        f"{temporal_subset}",
-                        f"{depth_range}",
-                        f"{limit}",
-                        f"{confirmation}",
+                        f"{subset_request}",
                     ]
                 )
                 + ")"
             )
             return
         download_opendap(
             login,
             password,
-            dataset_url,
-            output_path,
-            output_file,
-            variables,
-            geographical_subset,
-            temporal_subset,
-            depth_range,
-            limit,
-            confirmation,
+            subset_request,
         )
     elif protocol == MOTU_KEY:
         click.echo("download through MOTU")
-        if dry_run:
+        if subset_request.dry_run:
             print(
                 "download_motu("
                 + ", ".join(
                     [
-                        f"{dataset_url}",
-                        f"{dataset_id}",
                         f"{login}",
                         "HIDING_PASSWORD",
-                        f"{variables}",
-                        f"{geographical_subset}",
-                        f"{temporal_subset}",
-                        f"{depth_range}",
-                        f"{output_path}",
-                        f"{output_file}",
+                        f"{subset_request}",
                         "NOT_PRINTING_CATALOGUE",
                     ]
                 )
                 + ")"
             )
             return
         download_motu(
-            dataset_url,
-            dataset_id,
             login,
             password,
-            variables,
-            geographical_subset,
-            temporal_subset,
-            depth_range,
-            output_path,
-            output_file,
+            subset_request,
             catalogue=catalogue,
         )
     elif not protocol:
         raise KeyError(
-            f"The requested dataset '{dataset_id}' does not have "
+            f"The requested dataset '{subset_request.dataset_id}' does not have "
             f"{possible_protocols} url available"
         )
     else:
         raise KeyError(f"Protocol {protocol} not handled by subset command")
 
 
 if __name__ == "__main__":
```

### Comparing `copernicus_marine_client-0.4.0/copernicus_marine_client/download_functions/download_ftp.py` & `copernicus_marine_client-0.5.0/copernicus_marine_client/download_functions/download_ftp.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,47 @@
 import os
 from ftplib import FTP
 from multiprocessing.pool import ThreadPool
 from typing import Any, Tuple
 
+import click
 from numpy import append, arange
 
+from copernicus_marine_client.catalogue_parser.request_structure import (
+    NativeRequest,
+)
+
 # /////////////////////////////
 # ---Using ftplib
 # /////////////////////////////
 
 
 def download_ftp(
     login: str,
     password: str,
-    no_directories: bool,
-    output_path: str,
-    host: str,
-    filenames_in: list[str],
-    filenames_out: list[str],
+    native_request: NativeRequest,
 ) -> str:
-
+    message, host, filenames_in = download_header(
+        [native_request.dataset_url], login, password
+    )
+    filenames_out = create_filenames_out(
+        filenames_in,
+        native_request.output_directory,
+        native_request.no_directories,
+    )
+    click.echo(message)
+    if native_request.show_outputnames:
+        click.echo("Output filenames:")
+        [click.echo(filename_out) for filename_out in filenames_out]
+    if not native_request.assume_yes:
+        click.confirm("Do you want to continue?", abort=True)
     filenames_out = create_filenames_out(
-        filenames_in, output_path, no_directories
+        filenames_in,
+        native_request.output_directory,
+        native_request.no_directories,
     )
     pool = ThreadPool()
     nfiles_per_process, nfiles = 1, len(filenames_in)
     indexes = append(
         arange(0, nfiles, nfiles_per_process, dtype=int),
         nfiles,
     )
@@ -172,19 +188,19 @@
             path_dict[host].append(path)
         else:
             path_dict[host] = [path]
     return path_dict
 
 
 def create_filenames_out(
-    filenames_in: list[str], output_path: str = "", no_directories=False
+    filenames_in: list[str], output_directory: str = "", no_directories=False
 ) -> list[str]:
     filenames_out = []
     for filename_in in filenames_in:
-        filename_out = f"{output_path}/"
+        filename_out = f"{output_directory}/"
         if no_directories:
             filenames_out += [filename_out + filename_in.split("/")[-1]]
         elif filename_in.startswith("Core/"):
             filenames_out += [filename_out + filename_in[len("Core/") :]]
     return filenames_out
```

### Comparing `copernicus_marine_client-0.4.0/pyproject.toml` & `copernicus_marine_client-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "copernicus-marine-client"
-version = "0.4.0"
+version = "0.5.0"
 description = ""
 authors = ["jsouchard <jsouchard@mercator-ocean.fr>"]
 readme = "README.md"
 packages = [{include = "copernicus_marine_client"}]
 
 [tool.poetry.dependencies]
 python = ">=3.9"
```

### Comparing `copernicus_marine_client-0.4.0/README.md` & `copernicus_marine_client-0.5.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,203 +1,169 @@
 # Copernicus Marine Service client
 
 A library to facilitate the access of Copernicus Marine Service products and datasets.
 
 ## Introduction
 
 This package allows to recover products and datasets information from Command Line Interface or with Python code,
-as well as download subsets through opendap protocol.
+as well as download subsets and native files.
 
 ## Command Line Interface (CLI)
 
 ### Command *describe*
 Retrieve information about products as JSON:
 
 ```
 > copernicus-marine describe
 {
   "products": [
     {
-      "bbox": [
-        "-25.00",
-        "75.00",
-        "70.00",
-        "86.00"
-      ],
-      "created": "2011-10-11",
-      "product_id": "SEAICE_ARC_PHY_L3M_NRT_011_017",
-      "temporal_extent": [
-        "2021-04-27",
-        null
-      ],
-      "thumbnail": "https://catalogue.marine.copernicus.eu/documents/IMG/SEAICE_ARC_PHY_L3M_NRT_011_017.png",
-      "title": "ARCTIC Ocean and Sea-Ice Sigma-Nought"
+      "title": "Antarctic Sea Ice Extent from Reanalysis",
+      "product_id": "ANTARCTIC_OMI_SI_extent",
+      "thumbnail_url": "https://catalogue.marine.copernicus.eu/documents/IMG/ANTARCTIC_OMI_SI_extent.png",
+      "production_center": "Mercator Oc\u00e9an International",
+      "creation_datetime": "2018-02-12",
+      "modified_datetime": "2018-02-12",
     }
     ...
   ]
 }
 ```
 
-Retrieve all information about products and datasets as JSON:
+Retrieve all information about datasets as JSON:
 
 ```
-> copernicus-marine describe --include-description --include-datasets --include-providers --include-keywords
+> copernicus-marine describe --include-datasets
 {
-  "products": {
-    "title": "ARCTIC Ocean and Sea-Ice Sigma-Nought",
-    "product_id": "SEAICE_ARC_PHY_L3M_NRT_011_017",
-    "thumbnail": "https://catalogue.marine.copernicus.eu/documents/IMG/SEAICE_ARC_PHY_L3M_NRT_011_017.png",
-    "description": "'''Short description:''' \nFor the Arctic Ocean  - multiple Sentinel-1 scenes, Sigma0 calibrated and noise-corrected, with individual geographical map projections over Svalbard and Greenland Sea regions.\n\n'''DOI (product) :'''   \nhttps://doi.org/10.48670/moi-00124",
-    "providers": [
-      {
-        "name": "OSI-METNO-OSLO-NO (SD)",
-        "roles": [
-          "pointOfContact"
-        ],
-        "url": null,
-        "email": "marine-servicedesk@met.no"
-      },
-      {
-        "name": "OSI-METNO-OSLO-NO (PM)",
-        "roles": [
-          "originator"
-        ],
-        "url": null,
-        "email": "cecilie.wettre@met.no"
-      },
-      {
-        "name": "OSI-METNO-OSLO-NO (WPL)",
-        "roles": [
-          "custodian"
-        ],
-        "url": null,
-        "email": "ositac-manager@met.no"
-      },
-      {
-        "name": "SIW-METNO-OSLO-NO",
-        "roles": [
-          "resourceProvider"
-        ],
-        "url": null,
-        "email": "ositac-prod@met.no"
-      },
-      {
-        "name": "SIW-METNO-OSLO-NO",
-        "roles": [
-          "distributor"
-        ],
-        "url": null,
-        "email": "cmems-tech@met.no"
-      }
-    ],
-    "created": "2011-10-11",
-    "bbox": [
-      "-25.00",
-      "75.00",
-      "70.00",
-      "86.00"
-    ],
-            "uri": "ftp://nrt.cmems-du.eu/Core/SEAICE_ARC_PHY_L3M_NRT_011_017/cmems_obs-si_arc_physic_nrt_L2-EW_PT1H-irr"
-          }
-        ]
-      }
+  "products": [
+    {
+      "title": "Antarctic Sea Ice Extent from Reanalysis",
+      "product_id": "ANTARCTIC_OMI_SI_extent",
+      "thumbnail_url": "https://catalogue.marine.copernicus.eu/documents/IMG/ANTARCTIC_OMI_SI_extent.png",
+      "production_center": "Mercator Oc\u00e9an International",
+      "creation_datetime": "2018-02-12",
+      "modified_datetime": "2018-02-12",
+      "datasets": [
+        {
+          "dataset_id": "antarctic_omi_si_extent",
+          "dataset_name": "antarctic_omi_si_extent",
+          "services": [
+            {
+              "protocol": "ftp",
+              "uri": "ftp://my.cmems-du.eu/Core/ANTARCTIC_OMI_SI_extent/antarctic_omi_si_extent"
+            }
+          ],
+          "variables": []
+        }
+      ]
+    },
     ...
-    ]
-  }
+  ]
 }
 
 ```
 
 Check out the help:
 
 ```
 > copernicus-marine describe --help
 Usage: copernicus-marine describe [OPTIONS]
 
 Options:
   --one-line             Output JSON on one line
   --include-description  Include product description in output
   --include-datasets     Include product dataset details in output
-  --include-providers    Include product provider details in output
   --include-keywords     Include product keyword details in output
   -c, --contains TEXT    Filter catalogue output. Returns products with
                          attributes matching a string token
   --overwrite-cache      Force to refresh the catalogue by overwriting the
                          local cache
   --help                 Show this message and exit.
 ```
 
 ### Command *subset*
 
 Download a dataset subset, based on dataset id, variable names and attributes slices:
 
 ```
-> copernicus-marine subset -p METOFFICE-GLO-SST-L4-NRT-OBS-SST-V2 -v analysed_sst -v sea_ice_fraction -t 2021-01-01 2021-01-03 -g 0.0 0.1 0.0 0.1
+> copernicus-marine subset -i METOFFICE-GLO-SST-L4-NRT-OBS-SST-V2 -v analysed_sst -v sea_ice_fraction -t 2021-01-01 - T 2021-01-03 -x 0.0 -X 0.1 -y 0.0 -Y 0.1
 
 < Login:
 < Password:
 < Trying to download as one file...
 ```
 
-File downloaded to ./{dataset_id}.nc if not specified otherwise (through -o/--output-path and -f/--output-file options).
+File downloaded to ./{dataset_id}.nc if not specified otherwise (through -o/--output-directory and -f/--output-filename options).
 
 Check out the help:
 
 ```
 > copernicus-marine subset --help
 
 Usage: copernicus-marine subset [OPTIONS]
 
-  Downloads subsets of datasets as NetCDF files taking into account the server
-  data query limit. A 'dataset-id' (can be found via the 'copernicus-marine
-  describe' command) is required.
+  Downloads subsets of datasets as NetCDF files.     Either one of 'dataset-
+  id' or 'dataset-url' is required     (can be found via the 'copernicus-
+  marine describe' command).
 
   Example:
 
     copernicus-marine subset --dataset-id METOFFICE-GLO-SST-L4-NRT-OBS-SST-V2
-    --variable analysed_sst --variable sea_ice_fraction --temporal-subset
-    2021-01-01 2021-01-02 --geographical-subset 0.0 0.1 0.0 0.1
+    --variable analysed_sst --variable sea_ice_fraction --start-datetime
+    2021-01-01 --end-datetime 2021-01-02 --minimal-longitude 0.0 --maximal-
+    longitude 0.1 --minimal-latitude 0.0 --maximal-latitude 0.1
 
     copernicus-marine subset -i METOFFICE-GLO-SST-L4-NRT-OBS-SST-V2 -v
-    analysed_sst   -v sea_ice_fraction -t 2021-01-01 2021-01-02 -g 0.0 0.1 0.0
-    0.1
+    analysed_sst   -v sea_ice_fraction -t 2021-01-01 -T 2021-01-02 -x 0.0 -X
+    0.1 -y 0.0 -Y 0.1
 
 Options:
-  -u, --dataset-url TEXT          The full dataset URL option is mutually
-                                  exclusive with dataset_id.
-  -i, --dataset-id TEXT           The dataset id option is mutually exclusive
-                                  with dataset_url.
+  -u, --dataset-url TEXT          The full dataset URL
+  -i, --dataset-id TEXT           The dataset id
   --login TEXT
   --password TEXT
   -v, --variable TEXT             Specify dataset variables
-  -g, --geographical-subset <FLOAT RANGE FLOAT RANGE FLOAT RANGE FLOAT RANGE>...
-                                  The geographical subset as minimal latitude,
-                                  maximal latitude, minimal longitude and
-                                  maximal longitude
-  -t, --temporal-subset <DATETIME DATETIME>...
-                                  The temporal subset as start datetime and
-                                  end datetime
-  -d, --depth-range <FLOAT RANGE FLOAT RANGE>...
-                                  The depth range in meters, if depth is a
-                                  dataset coordinate
-  -o, --output-path PATH          The destination path for the downloaded
+  -x, --minimal-longitude FLOAT RANGE
+                                  Minimal longitude for the subset
+                                  [-180<=x<=180]
+  -X, --maximal-longitude FLOAT RANGE
+                                  Maximal longitude for the subset
+                                  [-180<=x<=180]
+  -y, --minimal-latitude FLOAT RANGE
+                                  Minimal latitude for the subset
+                                  [-90<=x<=90]
+  -Y, --maximal-latitude FLOAT RANGE
+                                  Maximal latitude for the subset
+                                  [-90<=x<=90]
+  -z, --minimal-depth FLOAT RANGE
+                                  Minimal depth for the subset  [x>=0]
+  -Z, --maximal-depth FLOAT RANGE
+                                  Maximal depth for the subset  [x>=0]
+  -t, --start-datetime [%Y|%Y-%m-%d|%Y-%m-%dT%H:%M:%S|%Y-%m-%d %H:%M:%S]
+                                  The start datetime of the temporal subset
+  -T, --end-datetime [%Y|%Y-%m-%d|%Y-%m-%dT%H:%M:%S|%Y-%m-%d %H:%M:%S]
+                                  The end datetime of the temporal subset
+  -o, --output-directory PATH     The destination folder for the downloaded
                                   files. Default is the current directory
                                   [required]
-  -f, --output-file PATH          Concatenate the downloaded data in the given
+  -f, --output-filename PATH      Concatenate the downloaded data in the given
                                   file name (under the output path)
-  -l, --limit INTEGER             Specify the download size limit (in MB) of
-                                  the Opendap server if it can't be provided
-                                  by the message error
-  --confirmation                  Print dataset metadata and ask for
-                                  confirmation before download
-  --force-protocol [WWW:OPENDAP|MYO:MOTU-SUB]
+  --assume-yes                    Flag to skip confirmation before download
+  --force-protocol [opendap|motu]
                                   Force download through one of the available
                                   protocols
   --dry-run                       Flag to specify NOT to send the request to
                                   external server. Returns the request instead
+  --request-file PATH             Option to pass a filename corresponding to a
+                                  file containg CLI arguments. The file MUST
+                                  follow the structure of dataclass
+                                  'SubsetRequest'. ANY PARAMETER SPECIFIED
+                                  ASIDE FROM FILE WILL NOT BE TAKEN INTO
+                                  CONSIDERATION FOR THE REQUEST IF FILE IS
+                                  SPECIFIED.
   --help                          Show this message and exit.
 ```
 
 ### Command *native*
 
 Download a native file (or files), based on dataset id or path to files:
 
@@ -250,31 +216,36 @@
     cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m
 
     copernicus-marine native -nd -o data_folder --dataset-url
     ftp://my.cmems-du.eu/Core/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-
     pft_myint_7km-3D-diato_P1M-m
 
 Options:
-  -u, --dataset-url TEXT  Path to the data files option is mutually exclusive
-                          with dataset_id.
-  -i, --dataset-id TEXT   The dataset id option is mutually exclusive with
-                          dataset_url.
+  -u, --dataset-url TEXT       Path to the data files
+  -i, --dataset-id TEXT        The dataset id
   --login TEXT
   --password TEXT
-  -nd, --no-directories   Option to not recreate folder hierarchy in ouput
-                          directory.
-  --show-outputnames      Option to display the names of the output files
-                          before download.
-  -o, --output-path PATH  The destination path for the downloaded files.
-                          Default is the current directory  [required]
-  --no-confirmation       Ask for confirmation before download, after header
-                          display
-  --dry-run               Flag to specify NOT to send the request to external
-                          server. Returns the request instead
-  --help                  Show this message and exit.
+  -nd, --no-directories        Option to not recreate folder hierarchy in
+                               ouput directory.
+  --show-outputnames           Option to display the names of the output files
+                               before download.
+  -o, --output-directory PATH  The destination directory for the downloaded
+                               files. Default is the current directory
+                               [required]
+  --assume-yes                 Whether to ask for confirmation before
+                               download, after header display. If 'True',
+                               skips confirmation.
+  --dry-run                    Flag to specify NOT to send the request to
+                               external server. Returns the request instead
+  --request-file PATH          Option to pass a file containg CLI arguments.
+                               The file MUST follow the structure of dataclass
+                               'SubsetRequest'. ANY PARAMETER SPECIFIED ASIDE
+                               FROM FILE WILL NOT BE TAKEN INTO CONSIDERATION
+                               FOR THE REQUEST IF FILE IS SPECIFIED.
+  --help                       Show this message and exit.
 ```
 
 ## Installation
 
 Using pip, for example:
 ```
 pip install copernicus-marine-client
@@ -284,7 +255,32 @@
 This module is organized around two capabilities:
 - a catalogue, parsed from web requests, that contains informations on the available datasets
 - a downloader, to simplify the download of dataset files or subsets
 
 The catalogue can be displayed by the user and is used by the downloader to link the user
 requests with files or subset of files to retrieve.
 The downloader will help the user download the needed datasets.
+
+A rigid format, specified in "request_structure.py" is used to ensure conformity of the information passed between the CLI command and the python functions.
+
+For subset command, the format is:
+
+```
+@dataclass
+class SubsetRequest:
+    dataset_url: Optional[str] = None
+    dataset_id: Optional[str] = None
+    variables: Optional[List[str]] = None
+    minimal_longitude: Optional[float] = None
+    maximal_longitude: Optional[float] = None
+    minimal_latitude: Optional[float] = None
+    maximal_latitude: Optional[float] = None
+    minimal_depth: Optional[float] = None
+    maximal_depth: Optional[float] = None
+    start_datetime: Optional[datetime] = None
+    end_datetime: Optional[datetime] = None
+    output_directory: Optional[str] = None
+    output_filename: Optional[str] = None
+    assume_yes: Optional[bool] = None
+    force_protocol: Optional[str] = None
+    dry_run: Optional[bool] = None
+```
```

### Comparing `copernicus_marine_client-0.4.0/setup.py` & `copernicus_marine_client-0.5.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -22,17 +22,17 @@
 
 entry_points = \
 {'console_scripts': ['copernicus-marine = '
                      'copernicus_marine_client.command_line_interface.copernicus_marine:command_line_interface']}
 
 setup_kwargs = {
     'name': 'copernicus-marine-client',
-    'version': '0.4.0',
+    'version': '0.5.0',
     'description': '',
-    'long_description': '# Copernicus Marine Service client\n\nA library to facilitate the access of Copernicus Marine Service products and datasets.\n\n## Introduction\n\nThis package allows to recover products and datasets information from Command Line Interface or with Python code,\nas well as download subsets through opendap protocol.\n\n## Command Line Interface (CLI)\n\n### Command *describe*\nRetrieve information about products as JSON:\n\n```\n> copernicus-marine describe\n{\n  "products": [\n    {\n      "bbox": [\n        "-25.00",\n        "75.00",\n        "70.00",\n        "86.00"\n      ],\n      "created": "2011-10-11",\n      "product_id": "SEAICE_ARC_PHY_L3M_NRT_011_017",\n      "temporal_extent": [\n        "2021-04-27",\n        null\n      ],\n      "thumbnail": "https://catalogue.marine.copernicus.eu/documents/IMG/SEAICE_ARC_PHY_L3M_NRT_011_017.png",\n      "title": "ARCTIC Ocean and Sea-Ice Sigma-Nought"\n    }\n    ...\n  ]\n}\n```\n\nRetrieve all information about products and datasets as JSON:\n\n```\n> copernicus-marine describe --include-description --include-datasets --include-providers --include-keywords\n{\n  "products": {\n    "title": "ARCTIC Ocean and Sea-Ice Sigma-Nought",\n    "product_id": "SEAICE_ARC_PHY_L3M_NRT_011_017",\n    "thumbnail": "https://catalogue.marine.copernicus.eu/documents/IMG/SEAICE_ARC_PHY_L3M_NRT_011_017.png",\n    "description": "\'\'\'Short description:\'\'\' \\nFor the Arctic Ocean  - multiple Sentinel-1 scenes, Sigma0 calibrated and noise-corrected, with individual geographical map projections over Svalbard and Greenland Sea regions.\\n\\n\'\'\'DOI (product) :\'\'\'   \\nhttps://doi.org/10.48670/moi-00124",\n    "providers": [\n      {\n        "name": "OSI-METNO-OSLO-NO (SD)",\n        "roles": [\n          "pointOfContact"\n        ],\n        "url": null,\n        "email": "marine-servicedesk@met.no"\n      },\n      {\n        "name": "OSI-METNO-OSLO-NO (PM)",\n        "roles": [\n          "originator"\n        ],\n        "url": null,\n        "email": "cecilie.wettre@met.no"\n      },\n      {\n        "name": "OSI-METNO-OSLO-NO (WPL)",\n        "roles": [\n          "custodian"\n        ],\n        "url": null,\n        "email": "ositac-manager@met.no"\n      },\n      {\n        "name": "SIW-METNO-OSLO-NO",\n        "roles": [\n          "resourceProvider"\n        ],\n        "url": null,\n        "email": "ositac-prod@met.no"\n      },\n      {\n        "name": "SIW-METNO-OSLO-NO",\n        "roles": [\n          "distributor"\n        ],\n        "url": null,\n        "email": "cmems-tech@met.no"\n      }\n    ],\n    "created": "2011-10-11",\n    "bbox": [\n      "-25.00",\n      "75.00",\n      "70.00",\n      "86.00"\n    ],\n            "uri": "ftp://nrt.cmems-du.eu/Core/SEAICE_ARC_PHY_L3M_NRT_011_017/cmems_obs-si_arc_physic_nrt_L2-EW_PT1H-irr"\n          }\n        ]\n      }\n    ...\n    ]\n  }\n}\n\n```\n\nCheck out the help:\n\n```\n> copernicus-marine describe --help\nUsage: copernicus-marine describe [OPTIONS]\n\nOptions:\n  --one-line             Output JSON on one line\n  --include-description  Include product description in output\n  --include-datasets     Include product dataset details in output\n  --include-providers    Include product provider details in output\n  --include-keywords     Include product keyword details in output\n  -c, --contains TEXT    Filter catalogue output. Returns products with\n                         attributes matching a string token\n  --overwrite-cache      Force to refresh the catalogue by overwriting the\n                         local cache\n  --help                 Show this message and exit.\n```\n\n### Command *subset*\n\nDownload a dataset subset, based on dataset id, variable names and attributes slices:\n\n```\n> copernicus-marine subset -p METOFFICE-GLO-SST-L4-NRT-OBS-SST-V2 -v analysed_sst -v sea_ice_fraction -t 2021-01-01 2021-01-03 -g 0.0 0.1 0.0 0.1\n\n< Login:\n< Password:\n< Trying to download as one file...\n```\n\nFile downloaded to ./{dataset_id}.nc if not specified otherwise (through -o/--output-path and -f/--output-file options).\n\nCheck out the help:\n\n```\n> copernicus-marine subset --help\n\nUsage: copernicus-marine subset [OPTIONS]\n\n  Downloads subsets of datasets as NetCDF files taking into account the server\n  data query limit. A \'dataset-id\' (can be found via the \'copernicus-marine\n  describe\' command) is required.\n\n  Example:\n\n    copernicus-marine subset --dataset-id METOFFICE-GLO-SST-L4-NRT-OBS-SST-V2\n    --variable analysed_sst --variable sea_ice_fraction --temporal-subset\n    2021-01-01 2021-01-02 --geographical-subset 0.0 0.1 0.0 0.1\n\n    copernicus-marine subset -i METOFFICE-GLO-SST-L4-NRT-OBS-SST-V2 -v\n    analysed_sst   -v sea_ice_fraction -t 2021-01-01 2021-01-02 -g 0.0 0.1 0.0\n    0.1\n\nOptions:\n  -u, --dataset-url TEXT          The full dataset URL option is mutually\n                                  exclusive with dataset_id.\n  -i, --dataset-id TEXT           The dataset id option is mutually exclusive\n                                  with dataset_url.\n  --login TEXT\n  --password TEXT\n  -v, --variable TEXT             Specify dataset variables\n  -g, --geographical-subset <FLOAT RANGE FLOAT RANGE FLOAT RANGE FLOAT RANGE>...\n                                  The geographical subset as minimal latitude,\n                                  maximal latitude, minimal longitude and\n                                  maximal longitude\n  -t, --temporal-subset <DATETIME DATETIME>...\n                                  The temporal subset as start datetime and\n                                  end datetime\n  -d, --depth-range <FLOAT RANGE FLOAT RANGE>...\n                                  The depth range in meters, if depth is a\n                                  dataset coordinate\n  -o, --output-path PATH          The destination path for the downloaded\n                                  files. Default is the current directory\n                                  [required]\n  -f, --output-file PATH          Concatenate the downloaded data in the given\n                                  file name (under the output path)\n  -l, --limit INTEGER             Specify the download size limit (in MB) of\n                                  the Opendap server if it can\'t be provided\n                                  by the message error\n  --confirmation                  Print dataset metadata and ask for\n                                  confirmation before download\n  --force-protocol [WWW:OPENDAP|MYO:MOTU-SUB]\n                                  Force download through one of the available\n                                  protocols\n  --dry-run                       Flag to specify NOT to send the request to\n                                  external server. Returns the request instead\n  --help                          Show this message and exit.\n```\n\n### Command *native*\n\nDownload a native file (or files), based on dataset id or path to files:\n\nExample:\n```\n> copernicus-marine native -u ftp://my.cmems-du.eu/Core/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/\n\n< Login:\n< Password:\n< You requested the download of the following files:\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202207.nc - 3.27 MB\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202208.nc - 3.29 MB\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202209.nc - 3.28 MB\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202210.nc - 3.26 MB\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202211.nc - 3.26 MB\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202212.nc - 3.26 MB\n\nTotal size of the download: 19.62 MB\n\n\nDo you want to continue? [y/N]:\n```\n\nFile(s) downloaded to ./{path}/{filename} if not specified otherwise:\n- "--output-path" specifies a directory to dump the files in\n- "--no-directories" to not recreate the folder structure\n\nIf not specified otherwise, after the header display with a summary of the request,\nthe user is asked for confirmation:\n- "--no-confirmation" to turn down the confirmation prompt\n- "--show-outputnames" to display the full paths of the outputs files\n\nCheck out the help:\n\n```\n> copernicus-marine native --help\n\nUsage: copernicus-marine native [OPTIONS]\n\n  Downloads native data files based on     dataset_id or datafiles url path.\n  The function fetches the files recursively if a folder path is passed as\n  url.     When provided a dataset id,     all the files in the corresponding\n  folder will be downloaded.\n\n      By default for any download request, a summary of the request result is\n      displayed to the user and a confirmation is asked.     This can be\n      turned down. Example:\n\n    copernicus-marine native -nd -o data_folder --dataset-id\n    cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m\n\n    copernicus-marine native -nd -o data_folder --dataset-url\n    ftp://my.cmems-du.eu/Core/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-\n    pft_myint_7km-3D-diato_P1M-m\n\nOptions:\n  -u, --dataset-url TEXT  Path to the data files option is mutually exclusive\n                          with dataset_id.\n  -i, --dataset-id TEXT   The dataset id option is mutually exclusive with\n                          dataset_url.\n  --login TEXT\n  --password TEXT\n  -nd, --no-directories   Option to not recreate folder hierarchy in ouput\n                          directory.\n  --show-outputnames      Option to display the names of the output files\n                          before download.\n  -o, --output-path PATH  The destination path for the downloaded files.\n                          Default is the current directory  [required]\n  --no-confirmation       Ask for confirmation before download, after header\n                          display\n  --dry-run               Flag to specify NOT to send the request to external\n                          server. Returns the request instead\n  --help                  Show this message and exit.\n```\n\n## Installation\n\nUsing pip, for example:\n```\npip install copernicus-marine-client\n```\n## Technical details\n\nThis module is organized around two capabilities:\n- a catalogue, parsed from web requests, that contains informations on the available datasets\n- a downloader, to simplify the download of dataset files or subsets\n\nThe catalogue can be displayed by the user and is used by the downloader to link the user\nrequests with files or subset of files to retrieve.\nThe downloader will help the user download the needed datasets.\n',
+    'long_description': '# Copernicus Marine Service client\n\nA library to facilitate the access of Copernicus Marine Service products and datasets.\n\n## Introduction\n\nThis package allows to recover products and datasets information from Command Line Interface or with Python code,\nas well as download subsets and native files.\n\n## Command Line Interface (CLI)\n\n### Command *describe*\nRetrieve information about products as JSON:\n\n```\n> copernicus-marine describe\n{\n  "products": [\n    {\n      "title": "Antarctic Sea Ice Extent from Reanalysis",\n      "product_id": "ANTARCTIC_OMI_SI_extent",\n      "thumbnail_url": "https://catalogue.marine.copernicus.eu/documents/IMG/ANTARCTIC_OMI_SI_extent.png",\n      "production_center": "Mercator Oc\\u00e9an International",\n      "creation_datetime": "2018-02-12",\n      "modified_datetime": "2018-02-12",\n    }\n    ...\n  ]\n}\n```\n\nRetrieve all information about datasets as JSON:\n\n```\n> copernicus-marine describe --include-datasets\n{\n  "products": [\n    {\n      "title": "Antarctic Sea Ice Extent from Reanalysis",\n      "product_id": "ANTARCTIC_OMI_SI_extent",\n      "thumbnail_url": "https://catalogue.marine.copernicus.eu/documents/IMG/ANTARCTIC_OMI_SI_extent.png",\n      "production_center": "Mercator Oc\\u00e9an International",\n      "creation_datetime": "2018-02-12",\n      "modified_datetime": "2018-02-12",\n      "datasets": [\n        {\n          "dataset_id": "antarctic_omi_si_extent",\n          "dataset_name": "antarctic_omi_si_extent",\n          "services": [\n            {\n              "protocol": "ftp",\n              "uri": "ftp://my.cmems-du.eu/Core/ANTARCTIC_OMI_SI_extent/antarctic_omi_si_extent"\n            }\n          ],\n          "variables": []\n        }\n      ]\n    },\n    ...\n  ]\n}\n\n```\n\nCheck out the help:\n\n```\n> copernicus-marine describe --help\nUsage: copernicus-marine describe [OPTIONS]\n\nOptions:\n  --one-line             Output JSON on one line\n  --include-description  Include product description in output\n  --include-datasets     Include product dataset details in output\n  --include-keywords     Include product keyword details in output\n  -c, --contains TEXT    Filter catalogue output. Returns products with\n                         attributes matching a string token\n  --overwrite-cache      Force to refresh the catalogue by overwriting the\n                         local cache\n  --help                 Show this message and exit.\n```\n\n### Command *subset*\n\nDownload a dataset subset, based on dataset id, variable names and attributes slices:\n\n```\n> copernicus-marine subset -i METOFFICE-GLO-SST-L4-NRT-OBS-SST-V2 -v analysed_sst -v sea_ice_fraction -t 2021-01-01 - T 2021-01-03 -x 0.0 -X 0.1 -y 0.0 -Y 0.1\n\n< Login:\n< Password:\n< Trying to download as one file...\n```\n\nFile downloaded to ./{dataset_id}.nc if not specified otherwise (through -o/--output-directory and -f/--output-filename options).\n\nCheck out the help:\n\n```\n> copernicus-marine subset --help\n\nUsage: copernicus-marine subset [OPTIONS]\n\n  Downloads subsets of datasets as NetCDF files.     Either one of \'dataset-\n  id\' or \'dataset-url\' is required     (can be found via the \'copernicus-\n  marine describe\' command).\n\n  Example:\n\n    copernicus-marine subset --dataset-id METOFFICE-GLO-SST-L4-NRT-OBS-SST-V2\n    --variable analysed_sst --variable sea_ice_fraction --start-datetime\n    2021-01-01 --end-datetime 2021-01-02 --minimal-longitude 0.0 --maximal-\n    longitude 0.1 --minimal-latitude 0.0 --maximal-latitude 0.1\n\n    copernicus-marine subset -i METOFFICE-GLO-SST-L4-NRT-OBS-SST-V2 -v\n    analysed_sst   -v sea_ice_fraction -t 2021-01-01 -T 2021-01-02 -x 0.0 -X\n    0.1 -y 0.0 -Y 0.1\n\nOptions:\n  -u, --dataset-url TEXT          The full dataset URL\n  -i, --dataset-id TEXT           The dataset id\n  --login TEXT\n  --password TEXT\n  -v, --variable TEXT             Specify dataset variables\n  -x, --minimal-longitude FLOAT RANGE\n                                  Minimal longitude for the subset\n                                  [-180<=x<=180]\n  -X, --maximal-longitude FLOAT RANGE\n                                  Maximal longitude for the subset\n                                  [-180<=x<=180]\n  -y, --minimal-latitude FLOAT RANGE\n                                  Minimal latitude for the subset\n                                  [-90<=x<=90]\n  -Y, --maximal-latitude FLOAT RANGE\n                                  Maximal latitude for the subset\n                                  [-90<=x<=90]\n  -z, --minimal-depth FLOAT RANGE\n                                  Minimal depth for the subset  [x>=0]\n  -Z, --maximal-depth FLOAT RANGE\n                                  Maximal depth for the subset  [x>=0]\n  -t, --start-datetime [%Y|%Y-%m-%d|%Y-%m-%dT%H:%M:%S|%Y-%m-%d %H:%M:%S]\n                                  The start datetime of the temporal subset\n  -T, --end-datetime [%Y|%Y-%m-%d|%Y-%m-%dT%H:%M:%S|%Y-%m-%d %H:%M:%S]\n                                  The end datetime of the temporal subset\n  -o, --output-directory PATH     The destination folder for the downloaded\n                                  files. Default is the current directory\n                                  [required]\n  -f, --output-filename PATH      Concatenate the downloaded data in the given\n                                  file name (under the output path)\n  --assume-yes                    Flag to skip confirmation before download\n  --force-protocol [opendap|motu]\n                                  Force download through one of the available\n                                  protocols\n  --dry-run                       Flag to specify NOT to send the request to\n                                  external server. Returns the request instead\n  --request-file PATH             Option to pass a filename corresponding to a\n                                  file containg CLI arguments. The file MUST\n                                  follow the structure of dataclass\n                                  \'SubsetRequest\'. ANY PARAMETER SPECIFIED\n                                  ASIDE FROM FILE WILL NOT BE TAKEN INTO\n                                  CONSIDERATION FOR THE REQUEST IF FILE IS\n                                  SPECIFIED.\n  --help                          Show this message and exit.\n```\n\n### Command *native*\n\nDownload a native file (or files), based on dataset id or path to files:\n\nExample:\n```\n> copernicus-marine native -u ftp://my.cmems-du.eu/Core/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/\n\n< Login:\n< Password:\n< You requested the download of the following files:\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202207.nc - 3.27 MB\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202208.nc - 3.29 MB\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202209.nc - 3.28 MB\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202210.nc - 3.26 MB\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202211.nc - 3.26 MB\nCore/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m/2022/metoffice_foam1_amm7_NWS_DIATO_CPWC_mm202212.nc - 3.26 MB\n\nTotal size of the download: 19.62 MB\n\n\nDo you want to continue? [y/N]:\n```\n\nFile(s) downloaded to ./{path}/{filename} if not specified otherwise:\n- "--output-path" specifies a directory to dump the files in\n- "--no-directories" to not recreate the folder structure\n\nIf not specified otherwise, after the header display with a summary of the request,\nthe user is asked for confirmation:\n- "--no-confirmation" to turn down the confirmation prompt\n- "--show-outputnames" to display the full paths of the outputs files\n\nCheck out the help:\n\n```\n> copernicus-marine native --help\n\nUsage: copernicus-marine native [OPTIONS]\n\n  Downloads native data files based on     dataset_id or datafiles url path.\n  The function fetches the files recursively if a folder path is passed as\n  url.     When provided a dataset id,     all the files in the corresponding\n  folder will be downloaded.\n\n      By default for any download request, a summary of the request result is\n      displayed to the user and a confirmation is asked.     This can be\n      turned down. Example:\n\n    copernicus-marine native -nd -o data_folder --dataset-id\n    cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m\n\n    copernicus-marine native -nd -o data_folder --dataset-url\n    ftp://my.cmems-du.eu/Core/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-\n    pft_myint_7km-3D-diato_P1M-m\n\nOptions:\n  -u, --dataset-url TEXT       Path to the data files\n  -i, --dataset-id TEXT        The dataset id\n  --login TEXT\n  --password TEXT\n  -nd, --no-directories        Option to not recreate folder hierarchy in\n                               ouput directory.\n  --show-outputnames           Option to display the names of the output files\n                               before download.\n  -o, --output-directory PATH  The destination directory for the downloaded\n                               files. Default is the current directory\n                               [required]\n  --assume-yes                 Whether to ask for confirmation before\n                               download, after header display. If \'True\',\n                               skips confirmation.\n  --dry-run                    Flag to specify NOT to send the request to\n                               external server. Returns the request instead\n  --request-file PATH          Option to pass a file containg CLI arguments.\n                               The file MUST follow the structure of dataclass\n                               \'SubsetRequest\'. ANY PARAMETER SPECIFIED ASIDE\n                               FROM FILE WILL NOT BE TAKEN INTO CONSIDERATION\n                               FOR THE REQUEST IF FILE IS SPECIFIED.\n  --help                       Show this message and exit.\n```\n\n## Installation\n\nUsing pip, for example:\n```\npip install copernicus-marine-client\n```\n## Technical details\n\nThis module is organized around two capabilities:\n- a catalogue, parsed from web requests, that contains informations on the available datasets\n- a downloader, to simplify the download of dataset files or subsets\n\nThe catalogue can be displayed by the user and is used by the downloader to link the user\nrequests with files or subset of files to retrieve.\nThe downloader will help the user download the needed datasets.\n\nA rigid format, specified in "request_structure.py" is used to ensure conformity of the information passed between the CLI command and the python functions.\n\nFor subset command, the format is:\n\n```\n@dataclass\nclass SubsetRequest:\n    dataset_url: Optional[str] = None\n    dataset_id: Optional[str] = None\n    variables: Optional[List[str]] = None\n    minimal_longitude: Optional[float] = None\n    maximal_longitude: Optional[float] = None\n    minimal_latitude: Optional[float] = None\n    maximal_latitude: Optional[float] = None\n    minimal_depth: Optional[float] = None\n    maximal_depth: Optional[float] = None\n    start_datetime: Optional[datetime] = None\n    end_datetime: Optional[datetime] = None\n    output_directory: Optional[str] = None\n    output_filename: Optional[str] = None\n    assume_yes: Optional[bool] = None\n    force_protocol: Optional[str] = None\n    dry_run: Optional[bool] = None\n```\n',
     'author': 'jsouchard',
     'author_email': 'jsouchard@mercator-ocean.fr',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `copernicus_marine_client-0.4.0/PKG-INFO` & `copernicus_marine_client-0.5.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: copernicus-marine-client
-Version: 0.4.0
+Version: 0.5.0
 Summary: 
 Author: jsouchard
 Author-email: jsouchard@mercator-ocean.fr
 Requires-Python: >=3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -22,203 +22,169 @@
 # Copernicus Marine Service client
 
 A library to facilitate the access of Copernicus Marine Service products and datasets.
 
 ## Introduction
 
 This package allows to recover products and datasets information from Command Line Interface or with Python code,
-as well as download subsets through opendap protocol.
+as well as download subsets and native files.
 
 ## Command Line Interface (CLI)
 
 ### Command *describe*
 Retrieve information about products as JSON:
 
 ```
 > copernicus-marine describe
 {
   "products": [
     {
-      "bbox": [
-        "-25.00",
-        "75.00",
-        "70.00",
-        "86.00"
-      ],
-      "created": "2011-10-11",
-      "product_id": "SEAICE_ARC_PHY_L3M_NRT_011_017",
-      "temporal_extent": [
-        "2021-04-27",
-        null
-      ],
-      "thumbnail": "https://catalogue.marine.copernicus.eu/documents/IMG/SEAICE_ARC_PHY_L3M_NRT_011_017.png",
-      "title": "ARCTIC Ocean and Sea-Ice Sigma-Nought"
+      "title": "Antarctic Sea Ice Extent from Reanalysis",
+      "product_id": "ANTARCTIC_OMI_SI_extent",
+      "thumbnail_url": "https://catalogue.marine.copernicus.eu/documents/IMG/ANTARCTIC_OMI_SI_extent.png",
+      "production_center": "Mercator Oc\u00e9an International",
+      "creation_datetime": "2018-02-12",
+      "modified_datetime": "2018-02-12",
     }
     ...
   ]
 }
 ```
 
-Retrieve all information about products and datasets as JSON:
+Retrieve all information about datasets as JSON:
 
 ```
-> copernicus-marine describe --include-description --include-datasets --include-providers --include-keywords
+> copernicus-marine describe --include-datasets
 {
-  "products": {
-    "title": "ARCTIC Ocean and Sea-Ice Sigma-Nought",
-    "product_id": "SEAICE_ARC_PHY_L3M_NRT_011_017",
-    "thumbnail": "https://catalogue.marine.copernicus.eu/documents/IMG/SEAICE_ARC_PHY_L3M_NRT_011_017.png",
-    "description": "'''Short description:''' \nFor the Arctic Ocean  - multiple Sentinel-1 scenes, Sigma0 calibrated and noise-corrected, with individual geographical map projections over Svalbard and Greenland Sea regions.\n\n'''DOI (product) :'''   \nhttps://doi.org/10.48670/moi-00124",
-    "providers": [
-      {
-        "name": "OSI-METNO-OSLO-NO (SD)",
-        "roles": [
-          "pointOfContact"
-        ],
-        "url": null,
-        "email": "marine-servicedesk@met.no"
-      },
-      {
-        "name": "OSI-METNO-OSLO-NO (PM)",
-        "roles": [
-          "originator"
-        ],
-        "url": null,
-        "email": "cecilie.wettre@met.no"
-      },
-      {
-        "name": "OSI-METNO-OSLO-NO (WPL)",
-        "roles": [
-          "custodian"
-        ],
-        "url": null,
-        "email": "ositac-manager@met.no"
-      },
-      {
-        "name": "SIW-METNO-OSLO-NO",
-        "roles": [
-          "resourceProvider"
-        ],
-        "url": null,
-        "email": "ositac-prod@met.no"
-      },
-      {
-        "name": "SIW-METNO-OSLO-NO",
-        "roles": [
-          "distributor"
-        ],
-        "url": null,
-        "email": "cmems-tech@met.no"
-      }
-    ],
-    "created": "2011-10-11",
-    "bbox": [
-      "-25.00",
-      "75.00",
-      "70.00",
-      "86.00"
-    ],
-            "uri": "ftp://nrt.cmems-du.eu/Core/SEAICE_ARC_PHY_L3M_NRT_011_017/cmems_obs-si_arc_physic_nrt_L2-EW_PT1H-irr"
-          }
-        ]
-      }
+  "products": [
+    {
+      "title": "Antarctic Sea Ice Extent from Reanalysis",
+      "product_id": "ANTARCTIC_OMI_SI_extent",
+      "thumbnail_url": "https://catalogue.marine.copernicus.eu/documents/IMG/ANTARCTIC_OMI_SI_extent.png",
+      "production_center": "Mercator Oc\u00e9an International",
+      "creation_datetime": "2018-02-12",
+      "modified_datetime": "2018-02-12",
+      "datasets": [
+        {
+          "dataset_id": "antarctic_omi_si_extent",
+          "dataset_name": "antarctic_omi_si_extent",
+          "services": [
+            {
+              "protocol": "ftp",
+              "uri": "ftp://my.cmems-du.eu/Core/ANTARCTIC_OMI_SI_extent/antarctic_omi_si_extent"
+            }
+          ],
+          "variables": []
+        }
+      ]
+    },
     ...
-    ]
-  }
+  ]
 }
 
 ```
 
 Check out the help:
 
 ```
 > copernicus-marine describe --help
 Usage: copernicus-marine describe [OPTIONS]
 
 Options:
   --one-line             Output JSON on one line
   --include-description  Include product description in output
   --include-datasets     Include product dataset details in output
-  --include-providers    Include product provider details in output
   --include-keywords     Include product keyword details in output
   -c, --contains TEXT    Filter catalogue output. Returns products with
                          attributes matching a string token
   --overwrite-cache      Force to refresh the catalogue by overwriting the
                          local cache
   --help                 Show this message and exit.
 ```
 
 ### Command *subset*
 
 Download a dataset subset, based on dataset id, variable names and attributes slices:
 
 ```
-> copernicus-marine subset -p METOFFICE-GLO-SST-L4-NRT-OBS-SST-V2 -v analysed_sst -v sea_ice_fraction -t 2021-01-01 2021-01-03 -g 0.0 0.1 0.0 0.1
+> copernicus-marine subset -i METOFFICE-GLO-SST-L4-NRT-OBS-SST-V2 -v analysed_sst -v sea_ice_fraction -t 2021-01-01 - T 2021-01-03 -x 0.0 -X 0.1 -y 0.0 -Y 0.1
 
 < Login:
 < Password:
 < Trying to download as one file...
 ```
 
-File downloaded to ./{dataset_id}.nc if not specified otherwise (through -o/--output-path and -f/--output-file options).
+File downloaded to ./{dataset_id}.nc if not specified otherwise (through -o/--output-directory and -f/--output-filename options).
 
 Check out the help:
 
 ```
 > copernicus-marine subset --help
 
 Usage: copernicus-marine subset [OPTIONS]
 
-  Downloads subsets of datasets as NetCDF files taking into account the server
-  data query limit. A 'dataset-id' (can be found via the 'copernicus-marine
-  describe' command) is required.
+  Downloads subsets of datasets as NetCDF files.     Either one of 'dataset-
+  id' or 'dataset-url' is required     (can be found via the 'copernicus-
+  marine describe' command).
 
   Example:
 
     copernicus-marine subset --dataset-id METOFFICE-GLO-SST-L4-NRT-OBS-SST-V2
-    --variable analysed_sst --variable sea_ice_fraction --temporal-subset
-    2021-01-01 2021-01-02 --geographical-subset 0.0 0.1 0.0 0.1
+    --variable analysed_sst --variable sea_ice_fraction --start-datetime
+    2021-01-01 --end-datetime 2021-01-02 --minimal-longitude 0.0 --maximal-
+    longitude 0.1 --minimal-latitude 0.0 --maximal-latitude 0.1
 
     copernicus-marine subset -i METOFFICE-GLO-SST-L4-NRT-OBS-SST-V2 -v
-    analysed_sst   -v sea_ice_fraction -t 2021-01-01 2021-01-02 -g 0.0 0.1 0.0
-    0.1
+    analysed_sst   -v sea_ice_fraction -t 2021-01-01 -T 2021-01-02 -x 0.0 -X
+    0.1 -y 0.0 -Y 0.1
 
 Options:
-  -u, --dataset-url TEXT          The full dataset URL option is mutually
-                                  exclusive with dataset_id.
-  -i, --dataset-id TEXT           The dataset id option is mutually exclusive
-                                  with dataset_url.
+  -u, --dataset-url TEXT          The full dataset URL
+  -i, --dataset-id TEXT           The dataset id
   --login TEXT
   --password TEXT
   -v, --variable TEXT             Specify dataset variables
-  -g, --geographical-subset <FLOAT RANGE FLOAT RANGE FLOAT RANGE FLOAT RANGE>...
-                                  The geographical subset as minimal latitude,
-                                  maximal latitude, minimal longitude and
-                                  maximal longitude
-  -t, --temporal-subset <DATETIME DATETIME>...
-                                  The temporal subset as start datetime and
-                                  end datetime
-  -d, --depth-range <FLOAT RANGE FLOAT RANGE>...
-                                  The depth range in meters, if depth is a
-                                  dataset coordinate
-  -o, --output-path PATH          The destination path for the downloaded
+  -x, --minimal-longitude FLOAT RANGE
+                                  Minimal longitude for the subset
+                                  [-180<=x<=180]
+  -X, --maximal-longitude FLOAT RANGE
+                                  Maximal longitude for the subset
+                                  [-180<=x<=180]
+  -y, --minimal-latitude FLOAT RANGE
+                                  Minimal latitude for the subset
+                                  [-90<=x<=90]
+  -Y, --maximal-latitude FLOAT RANGE
+                                  Maximal latitude for the subset
+                                  [-90<=x<=90]
+  -z, --minimal-depth FLOAT RANGE
+                                  Minimal depth for the subset  [x>=0]
+  -Z, --maximal-depth FLOAT RANGE
+                                  Maximal depth for the subset  [x>=0]
+  -t, --start-datetime [%Y|%Y-%m-%d|%Y-%m-%dT%H:%M:%S|%Y-%m-%d %H:%M:%S]
+                                  The start datetime of the temporal subset
+  -T, --end-datetime [%Y|%Y-%m-%d|%Y-%m-%dT%H:%M:%S|%Y-%m-%d %H:%M:%S]
+                                  The end datetime of the temporal subset
+  -o, --output-directory PATH     The destination folder for the downloaded
                                   files. Default is the current directory
                                   [required]
-  -f, --output-file PATH          Concatenate the downloaded data in the given
+  -f, --output-filename PATH      Concatenate the downloaded data in the given
                                   file name (under the output path)
-  -l, --limit INTEGER             Specify the download size limit (in MB) of
-                                  the Opendap server if it can't be provided
-                                  by the message error
-  --confirmation                  Print dataset metadata and ask for
-                                  confirmation before download
-  --force-protocol [WWW:OPENDAP|MYO:MOTU-SUB]
+  --assume-yes                    Flag to skip confirmation before download
+  --force-protocol [opendap|motu]
                                   Force download through one of the available
                                   protocols
   --dry-run                       Flag to specify NOT to send the request to
                                   external server. Returns the request instead
+  --request-file PATH             Option to pass a filename corresponding to a
+                                  file containg CLI arguments. The file MUST
+                                  follow the structure of dataclass
+                                  'SubsetRequest'. ANY PARAMETER SPECIFIED
+                                  ASIDE FROM FILE WILL NOT BE TAKEN INTO
+                                  CONSIDERATION FOR THE REQUEST IF FILE IS
+                                  SPECIFIED.
   --help                          Show this message and exit.
 ```
 
 ### Command *native*
 
 Download a native file (or files), based on dataset id or path to files:
 
@@ -271,31 +237,36 @@
     cmems_mod_nws_bgc-pft_myint_7km-3D-diato_P1M-m
 
     copernicus-marine native -nd -o data_folder --dataset-url
     ftp://my.cmems-du.eu/Core/NWSHELF_MULTIYEAR_BGC_004_011/cmems_mod_nws_bgc-
     pft_myint_7km-3D-diato_P1M-m
 
 Options:
-  -u, --dataset-url TEXT  Path to the data files option is mutually exclusive
-                          with dataset_id.
-  -i, --dataset-id TEXT   The dataset id option is mutually exclusive with
-                          dataset_url.
+  -u, --dataset-url TEXT       Path to the data files
+  -i, --dataset-id TEXT        The dataset id
   --login TEXT
   --password TEXT
-  -nd, --no-directories   Option to not recreate folder hierarchy in ouput
-                          directory.
-  --show-outputnames      Option to display the names of the output files
-                          before download.
-  -o, --output-path PATH  The destination path for the downloaded files.
-                          Default is the current directory  [required]
-  --no-confirmation       Ask for confirmation before download, after header
-                          display
-  --dry-run               Flag to specify NOT to send the request to external
-                          server. Returns the request instead
-  --help                  Show this message and exit.
+  -nd, --no-directories        Option to not recreate folder hierarchy in
+                               ouput directory.
+  --show-outputnames           Option to display the names of the output files
+                               before download.
+  -o, --output-directory PATH  The destination directory for the downloaded
+                               files. Default is the current directory
+                               [required]
+  --assume-yes                 Whether to ask for confirmation before
+                               download, after header display. If 'True',
+                               skips confirmation.
+  --dry-run                    Flag to specify NOT to send the request to
+                               external server. Returns the request instead
+  --request-file PATH          Option to pass a file containg CLI arguments.
+                               The file MUST follow the structure of dataclass
+                               'SubsetRequest'. ANY PARAMETER SPECIFIED ASIDE
+                               FROM FILE WILL NOT BE TAKEN INTO CONSIDERATION
+                               FOR THE REQUEST IF FILE IS SPECIFIED.
+  --help                       Show this message and exit.
 ```
 
 ## Installation
 
 Using pip, for example:
 ```
 pip install copernicus-marine-client
@@ -306,7 +277,32 @@
 - a catalogue, parsed from web requests, that contains informations on the available datasets
 - a downloader, to simplify the download of dataset files or subsets
 
 The catalogue can be displayed by the user and is used by the downloader to link the user
 requests with files or subset of files to retrieve.
 The downloader will help the user download the needed datasets.
 
+A rigid format, specified in "request_structure.py" is used to ensure conformity of the information passed between the CLI command and the python functions.
+
+For subset command, the format is:
+
+```
+@dataclass
+class SubsetRequest:
+    dataset_url: Optional[str] = None
+    dataset_id: Optional[str] = None
+    variables: Optional[List[str]] = None
+    minimal_longitude: Optional[float] = None
+    maximal_longitude: Optional[float] = None
+    minimal_latitude: Optional[float] = None
+    maximal_latitude: Optional[float] = None
+    minimal_depth: Optional[float] = None
+    maximal_depth: Optional[float] = None
+    start_datetime: Optional[datetime] = None
+    end_datetime: Optional[datetime] = None
+    output_directory: Optional[str] = None
+    output_filename: Optional[str] = None
+    assume_yes: Optional[bool] = None
+    force_protocol: Optional[str] = None
+    dry_run: Optional[bool] = None
+```
+
```

