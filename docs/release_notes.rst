Version 0.5.0 `January 24, 2022`
----------------------------------

- Add support on 10x Visium spatial data

  - Read the data folder by ``read_input`` function with ``file_type="visium"`` option.

  - Write 10x Visium data to Zarr format by ``write_output`` function with output file name of ``.zarr.zip`` extension.

Version 0.4.1 `November 4, 2021`
----------------------------------

- Fix issues on ``UnimodalData`` object construction.

Version 0.4.0 `October 19, 2021`
---------------------------------

- Add ``obsp`` and ``varp`` fields to store graph representation in terms of square matrices.
- Allow copy from View of ``AnnData``.
- In ``MultimodalData``, add ``register_attr`` function to register an attribute of a specified type in ``obs`` or ``obsm`` fields. This can be useful for adding information like gene signatures, etc.

Version 0.3.1 `July 16, 2021`
-------------------------------

- For ``aggregate_matrices`` function, allow sample-specific filtration on minimum number of UMIs (``nUMI`` column in sample sheet) and minimum number of genes (``nGene`` column in sample sheet), which would overwrite the corresponding parameters of the function for these samples.

Version 0.3.0 `July 6, 2021`
-------------------------------

- Add support for composite list (e.g. ``[0, pd.DataFrame, np.ndarray]``) in ``data.uns`` field for Zarr read/write.

Version 0.2.14 `June 28, 2021`
-------------------------------

- Add parameter ``uns_white_list`` in ``filter_data`` function to keep QC statistics if needed.

Version 0.2.13 `June 24, 2021`
-------------------------------

- The ``aggregate_matrices`` function now accepts sample sheet in Python dictionary format besides a CSV file path string. See details in its description in API panel.

Version 0.2.12 `May 28, 2021`
-------------------------------

- Bug fix.

Version 0.2.11 `May 17, 2021`
-------------------------------

- Bug fix.

Version 0.2.10 `February 2, 2021`
----------------------------------

- Feature enhancement.

Version 0.2.9 `December 25, 2020`
-----------------------------------

- Fix a bug for caching percent mito rate.
- Improve `write_mtx` function.

Version 0.2.8 `December 7, 2020`
-----------------------------------

- Add support on loading ``loom`` file with Seurat-style cell barcode and feature key names.
- Bug fix: resolve an issue on count matrix dimension inconsistency with feature metadata on data aggregation, when last feature has ``0`` count across all cell barcodes. Thanks to `Mikhail Alperovich <misha.alperovich1@gmail.com>`_ for reporting this issue.
- Other bug fix and performance improvements.

Version 0.2.7 `October 13, 2020`
-----------------------------------

- Add support for Nanostring GeoMx data format.
- Fix bugs.

Version 0.2.6 `September 28, 2020`
-----------------------------------

Fix bug in SCP compatible output generation.

Version 0.2.5 `August 19, 2020`
--------------------------------
Adjustment for Pegasus command usage.

Version 0.2.2 `June 16th, 2020`
--------------------------------
Fix bugs in data aggregation.

Version 0.2.1 `June 8th, 2020`
--------------------------------
Fix bug in processing single ``h5`` file.

Version 0.2.0 `June 7th, 2020`
--------------------------------
Initial release.
