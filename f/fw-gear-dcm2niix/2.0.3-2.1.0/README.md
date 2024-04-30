# Comparing `tmp/fw_gear_dcm2niix-2.0.3-py3-none-any.whl.zip` & `tmp/fw_gear_dcm2niix-2.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 25488 bytes, number of entries: 15
--rw-r--r--  2.0 unx      192 b- defN 80-Jan-01 00:00 fw_gear_dcm2niix/__init__.py
+Zip file size: 26277 bytes, number of entries: 15
+-rw-r--r--  2.0 unx      187 b- defN 80-Jan-01 00:00 fw_gear_dcm2niix/__init__.py
 -rw-r--r--  2.0 unx       27 b- defN 80-Jan-01 00:00 fw_gear_dcm2niix/dcm2niix/__init__.py
 -rw-r--r--  2.0 unx    14361 b- defN 80-Jan-01 00:00 fw_gear_dcm2niix/dcm2niix/arrange.py
--rw-r--r--  2.0 unx     7642 b- defN 80-Jan-01 00:00 fw_gear_dcm2niix/dcm2niix/dcm2niix_run.py
+-rw-r--r--  2.0 unx     7388 b- defN 80-Jan-01 00:00 fw_gear_dcm2niix/dcm2niix/dcm2niix_run.py
 -rw-r--r--  2.0 unx     5646 b- defN 80-Jan-01 00:00 fw_gear_dcm2niix/dcm2niix/dcm2niix_utils.py
--rw-r--r--  2.0 unx     3542 b- defN 80-Jan-01 00:00 fw_gear_dcm2niix/dcm2niix/interfaces.py
+-rw-r--r--  2.0 unx     3543 b- defN 80-Jan-01 00:00 fw_gear_dcm2niix/dcm2niix/interfaces.py
 -rw-r--r--  2.0 unx     1240 b- defN 80-Jan-01 00:00 fw_gear_dcm2niix/dcm2niix/prepare.py
 -rw-r--r--  2.0 unx       24 b- defN 80-Jan-01 00:00 fw_gear_dcm2niix/utils/__init__.py
--rw-r--r--  2.0 unx    15016 b- defN 80-Jan-01 00:00 fw_gear_dcm2niix/utils/metadata.py
--rw-r--r--  2.0 unx     7175 b- defN 80-Jan-01 00:00 fw_gear_dcm2niix/utils/parse_config.py
--rw-r--r--  2.0 unx     6904 b- defN 80-Jan-01 00:00 fw_gear_dcm2niix/utils/resolve.py
--rw-r--r--  2.0 unx    14183 b- defN 80-Jan-01 00:00 fw_gear_dcm2niix-2.0.3.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 fw_gear_dcm2niix-2.0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx     1092 b- defN 80-Jan-01 00:00 fw_gear_dcm2niix-2.0.3.dist-info/LICENSE
-?rw-r--r--  2.0 unx     1354 b- defN 16-Jan-01 00:00 fw_gear_dcm2niix-2.0.3.dist-info/RECORD
-15 files, 78486 bytes uncompressed, 23212 bytes compressed:  70.4%
+-rw-r--r--  2.0 unx    15784 b- defN 80-Jan-01 00:00 fw_gear_dcm2niix/utils/metadata.py
+-rw-r--r--  2.0 unx     9413 b- defN 80-Jan-01 00:00 fw_gear_dcm2niix/utils/parse_config.py
+-rw-r--r--  2.0 unx     7159 b- defN 80-Jan-01 00:00 fw_gear_dcm2niix/utils/resolve.py
+-rw-r--r--  2.0 unx     1092 b- defN 80-Jan-01 00:00 fw_gear_dcm2niix-2.1.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx    14676 b- defN 80-Jan-01 00:00 fw_gear_dcm2niix-2.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 fw_gear_dcm2niix-2.1.0.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1354 b- defN 16-Jan-01 00:00 fw_gear_dcm2niix-2.1.0.dist-info/RECORD
+15 files, 81982 bytes uncompressed, 24001 bytes compressed:  70.7%
```

## zipnote {}

```diff
@@ -27,20 +27,20 @@
 
 Filename: fw_gear_dcm2niix/utils/parse_config.py
 Comment: 
 
 Filename: fw_gear_dcm2niix/utils/resolve.py
 Comment: 
 
-Filename: fw_gear_dcm2niix-2.0.3.dist-info/METADATA
+Filename: fw_gear_dcm2niix-2.1.0.dist-info/LICENSE
 Comment: 
 
-Filename: fw_gear_dcm2niix-2.0.3.dist-info/WHEEL
+Filename: fw_gear_dcm2niix-2.1.0.dist-info/METADATA
 Comment: 
 
-Filename: fw_gear_dcm2niix-2.0.3.dist-info/LICENSE
+Filename: fw_gear_dcm2niix-2.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: fw_gear_dcm2niix-2.0.3.dist-info/RECORD
+Filename: fw_gear_dcm2niix-2.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fw_gear_dcm2niix/__init__.py

```diff
@@ -1,8 +1,9 @@
 """The fw_gear_dcm2niix package."""
+
 from importlib.metadata import version
 
 try:
     __version__ = version(__package__)
 # pylint: disable-next=bare-except
-except:  # pragma: no cover
+except:  # noqa: E722
     pass
```

## fw_gear_dcm2niix/dcm2niix/dcm2niix_run.py

```diff
@@ -1,25 +1,23 @@
 """Function to implement dcm2niix."""
 
 import logging
 import os
-from distutils import util
 
 # from nipype.interfaces.dcm2nii import Dcm2niix
 from .interfaces import Dcm2niixEnhanced
 
 logging.getLogger("nipype.interface").setLevel("CRITICAL")
 log = logging.getLogger(__name__)
 
 
 def convert_directory(
     source_dir,
     output_dir,
     anonymize_bids=True,
-    bids_sidecar="y",
     comment="",
     compress_images="y",
     compression_level=6,
     convert_only_series="all",
     crop=False,
     filename="%f_%p_%t_%s",
     ignore_derived=False,
@@ -37,16 +35,14 @@
 
     Args:
         source_dir (str): The absolute path to the output directory containing
             the files from the input(s).
         output_dir (str): The absolute path to the output directory to place the
             converted results.
         anonymize_bids (bool): If true, anonymize sidecar.
-        bids_sidecar (str): Output sidecar; 'y'=yes, 'n'=no, 'o'=only
-            (whereby no NIfTI file will be generated).
         comment (str): If non-empty, store comment as NIfTI aux_file
             (up to 24 characters).
         compress_images (str): Gzip compress images; 'y'=yes, 'i'=internal,
             'n'=no, '3'=no,3D. If option '3' is chosen, the filename flag will
             be set to '-f %p_%s' to prevent overwriting files.
         compression_level (int): If compressing images, set the gz compression
             level: 1 (fastest) to 9 (smallest).
@@ -79,21 +75,19 @@
         converter = Dcm2niixEnhanced()
         log.info("Starting dcm2niix %s", converter.version)
         log.info("Submitting %d DICOMs.", len(os.listdir(source_dir)))
 
         converter.inputs.source_dir = source_dir
         converter.inputs.output_dir = output_dir
 
-        # dcm2niix command configurations for: anonymize_bids, bids_sidecar
-        if bids_sidecar == "o" or bool(util.strtobool(bids_sidecar)):
-            converter.inputs.bids_format = True
-            converter.inputs.anon_bids = anonymize_bids
-        else:
-            log.info("The BIDS sidecar file will not be generated.")
-            converter.inputs.bids_format = False
+        # Because we're setting up dcm2niix to run as bids_sidecar = y
+        # at this stage no matter what the actual config says
+        # (we deal with whether to retain nifti and/or sidecar later)...
+        converter.inputs.bids_format = True
+        converter.inputs.anon_bids = anonymize_bids
 
         # dcm2niix command configurations for: comment
         if comment and (len(comment) < 25):
             converter.inputs.comment = comment
 
         # dcm2niix command configurations for: compress nifti
         if str(compress_images) == "3":
```

## fw_gear_dcm2niix/dcm2niix/interfaces.py

```diff
@@ -1,11 +1,12 @@
 """The interfaces module.
 
 Temporary resolution to include mvec files in output.
 """
+
 import os
 from copy import deepcopy
 
 from nipype.interfaces.base import File, OutputMultiPath, traits
 from nipype.interfaces.dcm2nii import (
     Dcm2niix,
     Dcm2niixInputSpec,
```

## fw_gear_dcm2niix/utils/metadata.py

```diff
@@ -22,14 +22,15 @@
     work_dir,
     dcm2niix_input_dir=None,
     retain_sidecar=False,
     retain_nifti=True,
     output_nrrd=False,
     classification=None,
     modality=None,
+    save_sidecar_as_metadata=False,
 ):
     # pylint: disable=too-many-arguments
     """Generate file metadata from dcm2niix output.
 
         Using the BIDS json sidecar output from dcm2niix, generate file metadata
         (file.info.header.dicom) and set the classification (file.measurements)
         from the input configuration settings.
@@ -46,14 +47,15 @@
         dcm2niix_input_dir (str): The absolute path to a set of dicoms as input
             to dcm2niix.
         retain_sidecar (bool): If true, sidecar is retained in final output.
         retain_nifti (bool): If true, nifti is retained in final output.
         output_nrrd (bool): If true, export as NRRD instead of NIfTI.
         classification (dict): File classification, typically from gear config.
         modality (str): File modality, typically from gear config.
+        save_sidecar_as_metadata (bool): Whether to save sidecar info into file metadata
 
     Returns:
         metadata_file (str): The absolute path to the metadata file generated.
 
     """
     # pylint: disable=duplicate-code
     metadata = capture(
@@ -61,14 +63,15 @@
         output_sidecar_files,
         dcm2niix_input_dir=dcm2niix_input_dir,
         retain_sidecar=retain_sidecar,
         retain_nifti=retain_nifti,
         output_nrrd=output_nrrd,
         classification=classification,
         modality=modality,
+        save_sidecar_as_metadata=save_sidecar_as_metadata,
     )
     # pylint: enable=duplicate-code
 
     metadata_file = create_file(metadata, work_dir)
 
     log.info("Metadata generation completed successfully.")
     metadata_formatted = pprint.pformat(metadata)
@@ -82,14 +85,15 @@
     output_sidecar_files,
     dcm2niix_input_dir=None,
     retain_sidecar=True,
     retain_nifti=True,
     output_nrrd=False,
     classification=None,
     modality=None,
+    save_sidecar_as_metadata=False,
 ):
     # pylint: disable=too-many-branches,too-many-statements,too-many-locals,too-many-arguments
     """Capture file metadata for each dcm2niix output.
 
         Using the BIDS json sidecar output from dcm2niix, generate file metadata
         (file.info.header.dicom) and set the classification (file.measurements)
         from the input configuration settings.
@@ -106,14 +110,15 @@
         dcm2niix_input_dir (str): The absolute path to a set of dicoms as input
             to dcm2niix.
         retain_sidecar (bool): If true, sidecar is retained in final output.
         retain_nifti (bool): If true, nifti is retained in final output.
         output_nrrd (bool): If true, export as NRRD instead of NIfTI.
         classification (dict): File classification, typically from gear config.
         modality (str): File modality, typically from gear config.
+        save_sidecar_as_metadata (bool): Whether to save sidecar info into file metadata
 
     Returns:
         metadata (dict): Structured metadata information for a given file set.
 
     """
     log.info("Capturing metadata.")
 
@@ -180,19 +185,25 @@
         else:
             log.info("Unable to capture additional metadata from DICOMs.")
 
         # Remove metadata with None value
         dicom_data = {k: v for k, v in dicom_data.items() if v is not None}
         log.debug("Structured metadata captured.")
 
+        # Maintain functionality for older BIDS workflow:
+        if save_sidecar_as_metadata:
+            metadata = {"sidecar_info": sidecar_info, "dicom_data": dicom_data}
+        else:
+            metadata = {"dicom_data": dicom_data}
+
         # Apply collated metadata to all associated files
 
         # Sidecar file
         filedata = create_file_metadata(
-            sidecar, "source code", classification, dicom_data, modality
+            sidecar, "source code", classification, metadata, modality
         )
         capture_metadata.append(filedata)
 
         # Data files
         # Split sidecar into the "root" name by removing .json suffix
         stem = sidecar.removesuffix(".json")
         for file in output_image_files:
@@ -208,31 +219,31 @@
             _, left = substr
             # pylint: enable=duplicate-code
 
             if retain_nifti:
                 # NIfTI
                 if left in [".nii.gz", ".nii"]:
                     filedata = create_file_metadata(
-                        file, "nifti", classification, dicom_data, modality
+                        file, "nifti", classification, metadata, modality
                     )
                     capture_metadata.append(filedata)
 
                 # bval, bvec, and mvec:
                 elif left in [".bval", ".bvec", ".mvec"]:
                     # (left[1:] removes the initial "." from the string)
                     filedata = create_file_metadata(
-                        file, left[1:], classification, dicom_data, modality
+                        file, left[1:], classification, metadata, modality
                     )
                     capture_metadata.append(filedata)
 
             if output_nrrd:
                 # NRRD
                 if left in [".raw.gz", ".nhdr", ".nrrd"]:
                     filedata = create_file_metadata(
-                        file, "nrrd", classification, dicom_data, modality
+                        file, "nrrd", classification, metadata, modality
                     )
                     capture_metadata.append(filedata)
 
     # If modality is not set, remove modality and classification from the metadata file
     if modality is None:
         for file in capture_metadata:
             file.pop("modality")
@@ -312,17 +323,17 @@
 
     try:
         dicom_data["PercentSampling"] = dicom_header.PercentSampling
     except AttributeError:
         dicom_data["PercentSampling"] = None
 
     try:
-        dicom_data[
-            "InPlanePhaseEncodingDirection"
-        ] = dicom_header.InPlanePhaseEncodingDirection
+        dicom_data["InPlanePhaseEncodingDirection"] = (
+            dicom_header.InPlanePhaseEncodingDirection
+        )
     except AttributeError:
         dicom_data["InPlanePhaseEncodingDirection"] = None
 
     try:
         dicom_data["AcquisitionMatrix"] = dicom_header.AcquisitionMatrix
     except AttributeError:
         dicom_data["AcquisitionMatrix"] = None
@@ -361,21 +372,25 @@
         dicom_data["ScanType"] = dicom_header[0x2005, 0x10A1].value
     except (AttributeError, KeyError):
         dicom_data["ScanType"] = None
 
     return dicom_data
 
 
-def create_file_metadata(filename, filetype, classification, dicom_data, modality):
+def create_file_metadata(filename, filetype, classification, metadata, modality):
     """Create a dictionary storing the file metadata."""
     filedata = {}
     filedata["name"] = Path(filename).name
     filedata["type"] = filetype
     filedata["classification"] = classification
-    filedata["info"] = {"header": {"dicom": dicom_data}}
+    if "sidecar_info" in metadata:
+        # If true, follow old behavior to be compatible with previous BIDS workflow
+        filedata["info"] = {**metadata["sidecar_info"], **metadata["dicom_data"]}
+    else:
+        filedata["info"] = {"header": {"dicom": metadata["dicom_data"]}}
     filedata["modality"] = modality
 
     return filedata
 
 
 def serialize_bytes(obj):
     """Serialize bytes."""
```

## fw_gear_dcm2niix/utils/parse_config.py

```diff
@@ -2,183 +2,253 @@
 
 import logging
 import os
 import pprint
 import re
 from pathlib import Path
 
+from flywheel_gear_toolkit import GearToolkitContext
+
 from fw_gear_dcm2niix.utils.metadata import rename_infile
 
 log = logging.getLogger(__name__)
 
 
-def generate_gear_args(gear_context, FLAG):
-    # pylint: disable=too-many-branches,too-many-statements
-    """Generate gear arguments for different stages indicated by the FLAG."""
+def generate_prep_args(gear_context: GearToolkitContext) -> dict:
+    """Generate gear arguments for the 'prepare' stage.
+
+    Args:
+        gear_context: Context and config needed to run gear
+
+    Returns:
+        dict: Gear arguments for the 'prepare' stage
+    """
     log.info("%s", 100 * "-")
-    log.info("Preparing arguments for gear stage >> %s", FLAG)
+    log.info("Preparing arguments for gear stage >> prepare")
 
-    if FLAG == "prepare":
-        infile = gear_context.get_input_path("dcm2niix_input")
+    infile = gear_context.get_input_path("dcm2niix_input")
+    try:
+        with open(infile, "r", encoding="utf-8") as f:
+            log.debug("%s opened from dcm2niix_input.", f)
+
+    except FileNotFoundError:
+        # Path separation in filename may cause downloaded filename to be altered
+        filename = (
+            gear_context.config_json.get("inputs", {})
+            .get("dcm2niix_input", {})
+            .get("location", {})
+            .get("name")
+        )
         try:
-            with open(infile, "r", encoding="utf-8") as f:
-                log.debug("%s opened from dcm2niix_input.", f)
-
-        except FileNotFoundError:
-            # Path separation in filename may cause downloaded filename to be altered
-            filename = (
-                gear_context.config_json.get("inputs", {})
-                .get("dcm2niix_input", {})
-                .get("location", {})
-                .get("name")
-            )
-            try:
-                if len(filename.split("/")) > 1:
-                    infile = (
-                        f"/flywheel/v0/input/dcm2niix_input/{filename.split('/')[-1]}"
-                    )
-
-                    with open(infile, "r", encoding="utf-8"):
-                        log.debug(
-                            "%s opened from path separated dcm2niix_input.", infile
-                        )
-            except (FileNotFoundError, AttributeError):
-                log.info(
-                    "Path to dcm2niix_input: %s",
-                    gear_context.get_input_path("dcm2niix_input"),
-                )
-                log.error(
-                    "Filename not understood from Gear context. Unable to open dcm2niix_input. Exiting."
-                )
-                os.sys.exit(1)
+            if len(filename.split("/")) > 1:
+                infile = f"/flywheel/v0/input/dcm2niix_input/{filename.split('/')[-1]}"
 
-        except UnicodeEncodeError:
+                with open(infile, "r", encoding="utf-8"):
+                    log.debug("%s opened from path separated dcm2niix_input.", infile)
+        except (FileNotFoundError, AttributeError):
             log.info(
                 "Path to dcm2niix_input: %s",
                 gear_context.get_input_path("dcm2niix_input"),
             )
             log.error(
                 "Filename not understood from Gear context. Unable to open dcm2niix_input. Exiting."
             )
             os.sys.exit(1)
 
-        # Rename infile if outfile is using infile folder
-        if (
-            bool(re.search("%f", gear_context.config["filename"]))
-            and gear_context.config["sanitize_filename"]
-        ):
-            infile = rename_infile(Path(infile))
-
-        gear_args = {
-            "infile": infile,
-            "work_dir": gear_context.work_dir,
-            "remove_incomplete_volumes": gear_context.config[
-                "remove_incomplete_volumes"
-            ],
-            "decompress_dicoms": gear_context.config["decompress_dicoms"],
-            "rec_infile": None,
-        }
-
-        if gear_context.get_input_path("rec_file_input"):
-            rec_infile = Path(gear_context.get_input_path("rec_file_input"))
-            if not rec_infile.is_file():
-                log.error(
-                    "Configuration for rec_infile_input is not a valid path. Exiting."
-                )
-                os.sys.exit(1)
-            # else:
-            gear_args["rec_infile"] = str(rec_infile)
-
-    elif FLAG == "dcm2niix":
-        # Notice the explicit 'y' for bids_sidecar, in order to capture metadata; the
-        # user-defined config option setting wil be considered during the gear resolve
-        # stage.
-        filename = gear_context.config["filename"]
-        # If filename is "%dicom%", use the dicom filename (without extension) as
-        # output filename:
-        if filename == "%dicom%":
-            filename = Path(gear_context.get_input_path("dcm2niix_input")).stem
-            # if there is still a ".dcm" extension, remove it:
-            filename = filename.removesuffix(".dcm")
-        filename = filename.replace(" ", "_")
-
-        comment = gear_context.config["comment"]
-        if len(comment) > 24:
+    except UnicodeEncodeError:
+        log.info(
+            "Path to dcm2niix_input: %s",
+            gear_context.get_input_path("dcm2niix_input"),
+        )
+        log.error(
+            "Filename not understood from Gear context. Unable to open dcm2niix_input. Exiting."
+        )
+        os.sys.exit(1)
+
+    # Rename infile if outfile is using infile folder
+    if (
+        bool(re.search("%f", gear_context.config["filename"]))
+        and gear_context.config["sanitize_filename"]
+    ):
+        infile = rename_infile(Path(infile))
+
+    gear_args = {
+        "infile": infile,
+        "work_dir": gear_context.work_dir,
+        "remove_incomplete_volumes": gear_context.config["remove_incomplete_volumes"],
+        "decompress_dicoms": gear_context.config["decompress_dicoms"],
+        "rec_infile": None,
+    }
+
+    if gear_context.get_input_path("rec_file_input"):
+        rec_infile = Path(gear_context.get_input_path("rec_file_input"))
+        if not rec_infile.is_file():
             log.error(
-                "The comment configuration option must be less than 25 characters. "
-                "You have entered %d characters. Please edit and resubmit Gear. "
-                "Exiting.",
-                len(comment),
+                "Configuration for rec_infile_input is not a valid path. Exiting."
             )
             os.sys.exit(1)
+        # else:
+        gear_args["rec_infile"] = str(rec_infile)
 
-        gear_args = {
-            "anonymize_bids": gear_context.config["anonymize_bids"],
-            "bids_sidecar": "y",
-            "comment": comment,
-            "compress_images": gear_context.config["compress_images"],
-            "compression_level": gear_context.config["compression_level"],
-            "convert_only_series": gear_context.config["convert_only_series"],
-            "crop": gear_context.config["crop"],
-            "filename": filename,
-            "ignore_derived": gear_context.config["ignore_derived"],
-            "ignore_errors": gear_context.config["ignore_errors"],
-            "lossless_scaling": gear_context.config["lossless_scaling"],
-            "merge2d": gear_context.config["merge2d"],
-            "output_nrrd": gear_context.config["output_nrrd"],
-            "philips_scaling": gear_context.config["philips_scaling"],
-            "single_file_mode": gear_context.config["single_file_mode"],
-            "text_notes_private": gear_context.config["text_notes_private"],
-            "verbose": gear_context.config["dcm2niix_verbose"],
-        }
-
-    elif FLAG == "resolve":
-        gear_args = {
-            "ignore_errors": gear_context.config["ignore_errors"],
-            "retain_sidecar": True,
-            "retain_nifti": True,
-            "output_nrrd": gear_context.config["output_nrrd"],
-            "classification": None,
-            "modality": None,
-        }
-
-        if (
-            gear_context.config["bids_sidecar"] == "o"
-            or gear_context.config["output_nrrd"]
-        ):
-            gear_args["retain_nifti"] = False
+    gear_args_formatted = pprint.pformat(gear_args)
+    log.info("Prepared gear stage arguments: \n\n%s\n", gear_args_formatted)
 
-        if gear_context.config["bids_sidecar"] == "n":
-            gear_args["retain_sidecar"] = False
+    return gear_args
 
-        try:
-            classification = (
-                gear_context.config_json.get("inputs", {})
-                .get("dcm2niix_input", {})
-                .get("object", {})
-                .get("classification")
-            )
-            # If modality is set and classification is not set, classification returned as {'Custom':[]}
-            # If modality and classification are not set, classification returned as {}
-            if classification not in ({}, {"Custom": []}):
-                gear_args["classification"] = classification
-        except KeyError:
-            log.info("Cannot determine classification from configuration.")
 
-        try:
-            gear_args["modality"] = (
-                gear_context.config_json.get("inputs", {})
-                .get("dcm2niix_input", {})
-                .get("object", {})
-                .get("modality")
+def generate_dcm2niix_args(gear_context: GearToolkitContext) -> dict:
+    """Generate gear arguments for the 'dcm2niix' stage.
+
+    Args:
+        gear_context: Context and config needed to run gear
+
+    Returns:
+        dict: Gear arguments for the 'dcm2niix' stage
+    """
+    log.info("%s", 100 * "-")
+    log.info("Preparing arguments for gear stage >> dcm2niix")
+
+    filename = gear_context.config["filename"]
+    # If filename is "%dicom%", use the dicom filename (without extension) as
+    # output filename:
+    if filename == "%dicom%":
+        filename = Path(gear_context.get_input_path("dcm2niix_input")).stem
+        # if there is still a ".dcm" extension, remove it:
+        filename = filename.removesuffix(".dcm")
+    filename = filename.replace(" ", "_")
+
+    comment = gear_context.config["comment"]
+    if len(comment) > 24:
+        log.error(
+            "The comment configuration option must be less than 25 characters. "
+            "You have entered %d characters. Please edit and resubmit Gear. "
+            "Exiting.",
+            len(comment),
+        )
+        os.sys.exit(1)
+
+    gear_args = {
+        "anonymize_bids": gear_context.config["anonymize_bids"],
+        "comment": comment,
+        "compress_images": gear_context.config["compress_images"],
+        "compression_level": gear_context.config["compression_level"],
+        "convert_only_series": gear_context.config["convert_only_series"],
+        "crop": gear_context.config["crop"],
+        "filename": filename,
+        "ignore_derived": gear_context.config["ignore_derived"],
+        "ignore_errors": gear_context.config["ignore_errors"],
+        "lossless_scaling": gear_context.config["lossless_scaling"],
+        "merge2d": gear_context.config["merge2d"],
+        "output_nrrd": gear_context.config["output_nrrd"],
+        "philips_scaling": gear_context.config["philips_scaling"],
+        "single_file_mode": gear_context.config["single_file_mode"],
+        "text_notes_private": gear_context.config["text_notes_private"],
+        "verbose": gear_context.config["dcm2niix_verbose"],
+    }
+
+    gear_args_formatted = pprint.pformat(gear_args)
+    log.info("Prepared gear stage arguments: \n\n%s\n", gear_args_formatted)
+
+    return gear_args
+
+
+def generate_resolve_args(gear_context: GearToolkitContext) -> dict:
+    """Generate gear arguments for the 'resolve' stage.
+
+    Args:
+        gear_context: Context and config needed to run gear
+
+    Returns:
+        dict: Gear arguments for the 'resolve' stage
+    """
+    log.info("%s", 100 * "-")
+    log.info("Preparing arguments for gear stage >> resolve")
+
+    gear_args = {
+        "ignore_errors": gear_context.config["ignore_errors"],
+        "bids_sidecar": gear_context.config["bids_sidecar"],
+        "retain_sidecar": True,
+        "retain_nifti": True,
+        "output_nrrd": gear_context.config["output_nrrd"],
+        "classification": None,
+        "modality": None,
+    }
+
+    if gear_context.config["bids_sidecar"] == "o" or gear_context.config["output_nrrd"]:
+        gear_args["retain_nifti"] = False
+
+    if gear_context.config["bids_sidecar"] == "n":
+        gear_args["retain_sidecar"] = False
+
+    # The save_sidecar_as_metadata arg exists to retain compatibility with
+    # the previous Flywheel BIDS workflow, which depends on the sidecar info
+    # being saved in file.info.
+    if gear_context.config["save_sidecar_as_metadata"] == "y":
+        # BIDS will ignore JSON sidecar. Sidecar will be stored as metadata.
+        gear_args["save_sidecar_as_metadata"] = True
+    elif gear_context.config["save_sidecar_as_metadata"] == "n":
+        # Default, expected behavior. BIDS will utilize JSON sidecar.
+        gear_args["save_sidecar_as_metadata"] = False
+    else:
+        # If arg not set, check to see if the project has old style BIDS metadata
+        container_id = gear_context.destination["id"]
+        container = gear_context.client.get(container_id)
+        project_id = container.parents["project"]
+        project = gear_context.client.get(project_id)
+        if "BIDS" in project.info:
+            if "Acknowledgements" in project.info["BIDS"]:
+                # Curated the old way
+                log.info(
+                    "Parent project identified as utilizing older BIDS "
+                    "curation workflow. Sidecar info will be stored in "
+                    "file.info for compatibility."
+                )
+                gear_args["save_sidecar_as_metadata"] = True
+            else:
+                log.info(
+                    "Parent project identified as utilizing current BIDS "
+                    "workflow. JSON sidecar info will not be saved as metadata."
+                )
+                gear_args["save_sidecar_as_metadata"] = False
+        else:
+            log.info(
+                "Parent project was not found to have BIDS info. "
+                "JSON sidecar info will not be saved as metadata."
             )
-        except KeyError:
-            log.info("Cannot determine modality from configuration.")
+            gear_args["save_sidecar_as_metadata"] = False
 
-        tag = gear_context.config.get("tag", "")
-        if tag != "":
-            gear_args["tag"] = tag
+    try:
+        classification = (
+            gear_context.config_json.get("inputs", {})
+            .get("dcm2niix_input", {})
+            .get("object", {})
+            .get("classification")
+        )
+        # If modality is set and classification is not set, classification returned as {'Custom':[]}
+        # If modality and classification are not set, classification returned as {}
+        if classification not in ({}, {"Custom": []}):
+            gear_args["classification"] = classification
+    except KeyError:
+        log.info("Cannot determine classification from configuration.")
+
+    try:
+        gear_args["modality"] = (
+            gear_context.config_json.get("inputs", {})
+            .get("dcm2niix_input", {})
+            .get("object", {})
+            .get("modality")
+        )
+    except KeyError:
+        log.info("Cannot determine modality from configuration.")
+
+    tag = gear_context.config.get("tag", "")
+    if tag != "":
+        gear_args["tag"] = tag
 
     gear_args_formatted = pprint.pformat(gear_args)
     log.info("Prepared gear stage arguments: \n\n%s\n", gear_args_formatted)
 
+    # bids_sidecar is useful to have logged for debugging, but doesn't need
+    # to be passed to the actual resolve stage.
+    del gear_args["bids_sidecar"]
+
     return gear_args
```

## fw_gear_dcm2niix/utils/resolve.py

```diff
@@ -17,14 +17,15 @@
     output_dir,
     ignore_errors=False,
     retain_sidecar=False,
     retain_nifti=True,
     output_nrrd=False,
     classification=None,
     modality=None,
+    save_sidecar_as_metadata=False,
 ):
     # pylint: disable=too-many-arguments,too-many-locals
     """Orchestrate resolution of gear, including metadata capture and file retention.
 
     Args:
         output_image_files (list): The absolute paths to converted image files to resolve.
             Typically these are NIfTI files, but can be the two files constituting the
@@ -36,14 +37,15 @@
             the metadata file generated is written to.
         dcm2niix_input_dir (str): The absolute path to the input directory to dcm2niix.
         retain_sidecar (bool): If true, sidecar is retained in final output.
         retain_nifti (bool): If true, NIfTI is retained in final output.
         output_nrrd (bool): If true, export as NRRD instead of NIfTI.
         classification (dict): File classification, typically from gear config.
         modality (str): File modality, typically from gear config.
+        save_sidecar_as_metadata (bool): Whether to save sidecar info into file metadata
 
     Returns:
         None
 
     """
     # Ignoring errors configuration option; move all files from work_dir to output_dir
     if ignore_errors is True:
@@ -57,14 +59,15 @@
                 work_dir,
                 dcm2niix_input_dir,
                 retain_sidecar=True,
                 retain_nifti=True,
                 output_nrrd=False,
                 classification=classification,
                 modality=modality,
+                save_sidecar_as_metadata=save_sidecar_as_metadata,
             )
 
         for item in os.listdir(work_dir):
             item_path = os.path.join(work_dir, item)
             if not os.path.isdir(item_path):
                 shutil.move(item_path, output_dir)
                 log.info("Moving %s to output directory for upload to Flywheel.", item)
@@ -78,14 +81,15 @@
             work_dir,
             dcm2niix_input_dir,
             retain_sidecar=retain_sidecar,
             retain_nifti=retain_nifti,
             output_nrrd=output_nrrd,
             classification=classification,
             modality=modality,
+            save_sidecar_as_metadata=save_sidecar_as_metadata,
         )
         # pylint: enable=duplicate-code
 
         # Retain gear outputs
         retain_gear_outputs(
             output_image_files,
             output_sidecar_files,
```

## Comparing `fw_gear_dcm2niix-2.0.3.dist-info/METADATA` & `fw_gear_dcm2niix-2.1.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: fw-gear-dcm2niix
-Version: 2.0.3
+Version: 2.1.0
 Summary: A Flywheel Gear for implementing Chris Rorden's dcm2niix for converting DICOM (or PAR/REC) to NIfTI (or NRRD).
 Home-page: https://gitlab.com/flywheel-io/scientific-solutions/gears/dcm2niix/
 License: Other
 Keywords: Flywheel,Gears
 Author: Flywheel
 Author-email: support@flywheel.io
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Requires-Dist: flywheel-gear-toolkit (>=0.6.10,<0.7.0)
-Requires-Dist: fw-file (==1.3.3)
-Requires-Dist: fw-gear-file-metadata-importer (>=1.2.5,<2.0.0)
+Requires-Dist: fw-file (>=3.0.1,<4.0.0)
+Requires-Dist: fw-gear-file-metadata-importer (>=1.4.0,<2.0.0)
 Requires-Dist: nibabel (>=3.2.0,<3.3.0)
 Requires-Dist: nipype (>=1.8.4,<1.9.0)
 Requires-Dist: numpy (>=1.13)
 Requires-Dist: pydicom (>=2.1.0,<3.0.0)
 Project-URL: Repository, https://gitlab.com/flywheel-io/scientific-solutions/gears/dcm2niix/
 Description-Content-Type: text/markdown
 
@@ -180,14 +181,19 @@
   - __Description__: Remove incomplete trailing volumes for 4D scans aborted mid-acquisition before dcm2niix conversion. Options: true, false (default).
   - __Default__: False
 - sanitize_filename
   - __Name__: sanitize_filename
   - __Type__: Boolean
   - __Description__: Sanitize filename by removing invalid characters.
   - __Default__: True
+- save_sidecar_as_metadata
+  - __Name__: save_sidecar_as_metadata
+  - __Type__: string
+  - __Description__: Whether to save sidecar information in `file.info` metadata to be compatible with previous BIDS workflow. Options: 'y'=yes, 'n'=no, or leave blank (default). If left blank, gear will check `project.info` and attempt to identify if the previous BIDS curation method is being utilized for the parent project.
+  - __Default__: ""
 - single_file_mode
   - __Name__: single_file_mode
   - __Type__: Boolean
   - __Description__: Single file mode, do not convert other images in the folder. Options: true, false (default).
   - __Default__: False
 - tag
   - __Name__: tag
```

## Comparing `fw_gear_dcm2niix-2.0.3.dist-info/LICENSE` & `fw_gear_dcm2niix-2.1.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `fw_gear_dcm2niix-2.0.3.dist-info/RECORD` & `fw_gear_dcm2niix-2.1.0.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-fw_gear_dcm2niix/__init__.py,sha256=YaB4aZxevqASxeO3okRaTHvCQVY6DS7BEGVymPgO2dQ,192
+fw_gear_dcm2niix/__init__.py,sha256=qZUBR5GjUYRN5I5YsLAlAfeFI469jnGgesk4G6OGpPQ,187
 fw_gear_dcm2niix/dcm2niix/__init__.py,sha256=gD5DzU4HJdzPQrsVL3sChft0ymhmdyDtqaPrG2AcX4U,27
 fw_gear_dcm2niix/dcm2niix/arrange.py,sha256=VwfF52hYLsAM5m-UaVoQ098VoTclGpr8vp6ksZHCWvE,14361
-fw_gear_dcm2niix/dcm2niix/dcm2niix_run.py,sha256=GMl_YzdPglMiWb_DRXD7bXqSCKtTXhw5Y2igtwJJAGY,7642
+fw_gear_dcm2niix/dcm2niix/dcm2niix_run.py,sha256=jzBp0OIG-C9v7-ganTM-iN30_LU4JMM8NvakWec4b3I,7388
 fw_gear_dcm2niix/dcm2niix/dcm2niix_utils.py,sha256=Bi7FVy2B4qeUJr_57FAM9OjizTRYeDDuLIvzoVEDpf8,5646
-fw_gear_dcm2niix/dcm2niix/interfaces.py,sha256=e_p9hf2G-fR94R8O_sgCN9PGgiLRvZWZhRkge5FgI34,3542
+fw_gear_dcm2niix/dcm2niix/interfaces.py,sha256=le6USl7visnS-HqKtOPjaGRqkUzBc5rffrgNeHXGrgY,3543
 fw_gear_dcm2niix/dcm2niix/prepare.py,sha256=SXB0Hglz6Y8L0yJ1h61YBFtAZMVtht1c59Iltz3O4II,1240
 fw_gear_dcm2niix/utils/__init__.py,sha256=JqFj1MIfZbijg-OcS_ho5QzMfpHEy2G-Pn95dFTlioM,24
-fw_gear_dcm2niix/utils/metadata.py,sha256=ipjsjmZke3xubty-AT73RmaeCOEnIPTTumA-epeBE7k,15016
-fw_gear_dcm2niix/utils/parse_config.py,sha256=EpsMRiAtvaqekciBEPRhX-VWb7QnyjIQbYGqrS9s6TA,7175
-fw_gear_dcm2niix/utils/resolve.py,sha256=geyQqxyA_U2LFK1pvZj-l5-g0E0WZrnOH9NBH4ywMNA,6904
-fw_gear_dcm2niix-2.0.3.dist-info/METADATA,sha256=OpQo3Eg80lsdU2C1FYRbXZXzSyIM8LAskMslDJJYXTs,14183
-fw_gear_dcm2niix-2.0.3.dist-info/WHEEL,sha256=vVCvjcmxuUltf8cYhJ0sJMRDLr1XsPuxEId8YDzbyCY,88
-fw_gear_dcm2niix-2.0.3.dist-info/LICENSE,sha256=NNC8xrLtqnhvmkJdOB71ctPp2jBi_2V5u9RzRVEpBcs,1092
-fw_gear_dcm2niix-2.0.3.dist-info/RECORD,,
+fw_gear_dcm2niix/utils/metadata.py,sha256=DzbFhY2J3vXSZdbHSOZRVtDt-Z-qMJE7qcWsyCnOBMo,15784
+fw_gear_dcm2niix/utils/parse_config.py,sha256=twPGXRx0ai0a5qVrn6skF7RDxjLCRQa-qMF0Zuh-sE0,9413
+fw_gear_dcm2niix/utils/resolve.py,sha256=xv9lDtNUNRXFMMD3Z3rdIzs5lk570O9sp1TOfLT8IYo,7159
+fw_gear_dcm2niix-2.1.0.dist-info/LICENSE,sha256=NNC8xrLtqnhvmkJdOB71ctPp2jBi_2V5u9RzRVEpBcs,1092
+fw_gear_dcm2niix-2.1.0.dist-info/METADATA,sha256=SX6f0iUeXlXstnWwsDEulHFclorNx6LKDYDSCSsq3IY,14676
+fw_gear_dcm2niix-2.1.0.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
+fw_gear_dcm2niix-2.1.0.dist-info/RECORD,,
```

