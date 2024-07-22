# asyncio
import time
import asyncio

balls = [1, 2, 3, 4, 5]
async def start_strongman(name, power):
    print(f'силач {name} начал соревноваия')
    time.sleep({power})
    print('силач поднял', balls(range(5)))

async def start_tournament():
    print('старт')
    task1 = asyncio.create_task(start_strongman('misha', 4))
    await task1
    task2 = asyncio.create_task(start_strongman('kolya', 5))
    await task2
    task3 = asyncio.create_task(start_strongman('igor', 6))
    await task3
    print("финиш")

start = time.time()
asyncio.run(start_tournament())
