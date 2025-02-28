deeplake.api.dataset
====================
.. currentmodule:: deeplake.api.dataset
.. class:: dataset
    
    .. staticmethod:: exists(path: Union[str, pathlib.Path], creds: Optional[dict] = None, token: Optional[str] = None) -> bool

        See :func:`deeplake.exists`.
    
    .. staticmethod:: empty(path: Union[str, pathlib.Path], overwrite: bool = False, public: bool = False, memory_cache_size: int = DEFAULT_MEMORY_CACHE_SIZE, local_cache_size: int = DEFAULT_LOCAL_CACHE_SIZE, creds: Optional[dict] = None, token: Optional[str] = None) -> Dataset

        See :func:`deeplake.empty`.
    
    .. staticmethod:: load(path: Union[str, pathlib.Path], read_only: Optional[bool] = None, memory_cache_size: int = DEFAULT_MEMORY_CACHE_SIZE, local_cache_size: int = DEFAULT_LOCAL_CACHE_SIZE, creds: Optional[dict] = None, token: Optional[str] = None, verbose: bool = True, access_method: str = "stream") -> Dataset

        See :func:`deeplake.load`.
    
    .. staticmethod:: rename(old_path: Union[str, pathlib.Path], new_path: Union[str, pathlib.Path], creds: Optional[dict] = None, token: Optional[str] = None) -> Dataset

        See :func:`deeplake.rename`.
    
    .. staticmethod:: delete(path: Union[str, pathlib.Path], force: bool = False, large_ok: bool = False, creds: Optional[dict] = None, token: Optional[str] = None, verbose: bool = False) -> None

        See :func:`deeplake.delete`.

    .. staticmethod:: like(dest: Union[str, pathlib.Path], src: Union[str, Dataset, pathlib.Path], tensors: Optional[List[str]] = None, overwrite: bool = False, creds: Optional[dict] = None, token: Optional[str] = None, public: bool = False) -> Dataset
        
        See :func:`deeplake.like`.
    
    .. staticmethod:: copy(src: Union[str, pathlib.Path, Dataset], dest: Union[str, pathlib.Path], tensors: Optional[List[str]] = None, overwrite: bool = False, src_creds=None, dest_creds=None, token=None, num_workers: int = 0, scheduler="threaded", progressbar=True)
        
        See :func:`deeplake.copy`.
    
    .. staticmethod:: deepcopy(src: Union[str, pathlib.Path], dest: Union[str, pathlib.Path], tensors: Optional[List[str]] = None, overwrite: bool = False, src_creds=None, dest_creds=None, token=None, num_workers: int = 0, scheduler="threaded", progressbar=True, public: bool = False, verbose: bool = True)

        See :func:`deeplake.deepcopy`.

    .. staticmethod:: connect(src_path: str, creds_key: str, dest_path: Optional[str], org_id: Optional[str], ds_name: Optional[str], token: Optional[str])

        See :func:`deeplake.connect`.
    
    .. staticmethod:: ingest(src: Union[str, pathlib.Path], dest: Union[str, pathlib.Path], images_compression: str = "auto", dest_creds: dict = None, progressbar: bool = True, summary: bool = True, **dataset_kwargs) -> Dataset

        See :func:`deeplake.ingest`.

    .. staticmethod:: ingest_coco(images_directory: Union[str, pathlib.Path], annotation_files: Union[str, pathlib.Path, List[str]], dest: Union[str, pathlib.Path], key_to_tensor_mapping: Optional[Dict] = None, file_to_group_mapping: Optional[Dict] = None, ignore_one_group: bool = False, ignore_keys: Optional[List[str]] = None, image_settings: Optional[Dict] = None, src_creds: Optional[Dict] = None, dest_creds: Optional[Dict] = None, inspect_limit: int = 1000000, progressbar: bool = True, num_workers: int = 0, **dataset_kwargs) -> Dataset

        See :func:`deeplake.ingest_coco`.
    
    .. staticmethod:: ingest_kaggle(tag: str, src: Union[str, pathlib.Path], dest: Union[str, pathlib.Path], exist_ok: bool = False, images_compression: str = "auto", dest_creds: dict = None, kaggle_credentials: dict = None, progressbar: bool = True, summary: bool = True, **dataset_kwargs) -> Dataset

        See :func:`deeplake.ingest_kaggle`.
    
    .. staticmethod:: ingest_dataframe(src, dest: Union[str, pathlib.Path], dest_creds: Optional[Dict] = None, progressbar: bool = True,**dataset_kwargs)

        See :func:`deeplake.ingest_dataframe`.
    
    .. staticmethod:: list(workspace: str = "", token: Optional[str] = None,) -> None

        See :func:`deeplake.list`.