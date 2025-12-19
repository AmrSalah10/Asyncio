# Asyncio Tutorial

A comprehensive guide and set of examples for mastering Python's `asyncio` library. This project covers everything from basic asynchronous tasks to real-world performance optimizations using threads and processes.

## Tutorial Parts

### 1. Basic Asyncio
- [1.async_normal.py](file:///d:/Studying/Github%20Repos/Ayncio/1.async_normal.py): Basic usage of `asyncio.create_task` and `await` for concurrent execution of coroutines.

### 2. Async with Threads and Processes
- [2.async_with_thread.py](file:///d:/Studying/Github%20Repos/Ayncio/2.async_with_thread.py): Demonstrates running blocking I/O bound tasks in threads using `asyncio.to_thread`.
- [3.async_with_process.py](file:///d:/Studying/Github%20Repos/Ayncio/3.async_with_process.py): Shows how to use `ProcessPoolExecutor` for CPU-bound tasks within an async loop.

### 3. Task Management
- [4.async_group_tasksk.py](file:///d:/Studying/Github%20Repos/Ayncio/4.async_group_tasksk.py): Comparing `asyncio.gather` with the newer (Python 3.11+) `asyncio.TaskGroup` for managing multiple tasks.

### 4. Real World Examples: Image Processing
These scripts demonstrate a practical scenario: downloading high-resolution images and performing edge detection.
- [5.real_examle_sync.py](file:///d:/Studying/Github%20Repos/Ayncio/5.real_examle_sync.py): The synchronous baseline using `requests` and serial processing.
- [6.real_examle_async.py](file:///d:/Studying/Github%20Repos/Ayncio/6.real_examle_async.py): Async version using `aiohttp`, `aiofiles`, and `ProcessPoolExecutor` for significantly better performance.
- [7.real_examle_async_v2.py](file:///d:/Studying/Github%20Repos/Ayncio/7.real_examle_async_v2.py): An alternative async version using `httpx` for modern async HTTP requests.

## Setup and Requirements
This project uses `uv` for dependency management.
### Requirements
- Python 3.11+
- `aiohttp`
- `aiofiles`
- `httpx`
- `requests`
- `Pillow` (PIL)

## References
This project was developed using the following tutorial as a reference:
- [Python Asyncio Tutorial](https://www.youtube.com/watch?v=oAkLSJNr5zY&list=PL-osiE80TeTt2d9bfVyTiXJA-UTHn6WwU&index=178)