# Comparing `tmp/arm_jupyter_kernel-1.0.8.tar.gz` & `tmp/arm_jupyter_kernel-1.1.0.tar.gz`

## Comparing `arm_jupyter_kernel-1.0.8.tar` & `arm_jupyter_kernel-1.1.0.tar`

### file list

```diff
@@ -1,20 +1,22 @@
--rwxr-xr-x   0        0        0       89 2020-02-02 00:00:00.000000 arm_jupyter_kernel-1.0.8/arm_kernel/__init__.py
--rwxr-xr-x   0        0        0      123 2020-02-02 00:00:00.000000 arm_jupyter_kernel-1.0.8/arm_kernel/__main__.py
--rwxr-xr-x   0        0        0     2898 2020-02-02 00:00:00.000000 arm_jupyter_kernel-1.0.8/arm_kernel/arm_kernel.py
--rwxr-xr-x   0        0        0     4664 2020-02-02 00:00:00.000000 arm_jupyter_kernel-1.0.8/arm_kernel/emulator.py
--rwxr-xr-x   0        0        0     2044 2020-02-02 00:00:00.000000 arm_jupyter_kernel-1.0.8/arm_kernel/install.py
--rwxr-xr-x   0        0        0       99 2020-02-02 00:00:00.000000 arm_jupyter_kernel-1.0.8/arm_kernel/kernel.json
--rwxr-xr-x   0        0        0    10640 2020-02-02 00:00:00.000000 arm_jupyter_kernel-1.0.8/arm_kernel/memory.py
--rwxr-xr-x   0        0        0     5166 2020-02-02 00:00:00.000000 arm_jupyter_kernel-1.0.8/arm_kernel/preprocessor.py
--rwxr-xr-x   0        0        0     9004 2020-02-02 00:00:00.000000 arm_jupyter_kernel-1.0.8/arm_kernel/registers.py
--rwxr-xr-x   0        0        0     6885 2020-02-02 00:00:00.000000 arm_jupyter_kernel-1.0.8/arm_kernel/view.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 arm_jupyter_kernel-1.0.8/arm_kernel/templates/__init__.py
--rwxr-xr-x   0        0        0      297 2020-02-02 00:00:00.000000 arm_jupyter_kernel-1.0.8/arm_kernel/templates/memory.py
--rwxr-xr-x   0        0        0      659 2020-02-02 00:00:00.000000 arm_jupyter_kernel-1.0.8/arm_kernel/templates/register.py
--rwxr-xr-x   0        0        0      546 2020-02-02 00:00:00.000000 arm_jupyter_kernel-1.0.8/arm_kernel/templates/stack.py
--rwxr-xr-x   0        0        0      224 2020-02-02 00:00:00.000000 arm_jupyter_kernel-1.0.8/.gitignore
--rwxr-xr-x   0        0        0    35821 2020-02-02 00:00:00.000000 arm_jupyter_kernel-1.0.8/LICENSE
--rwxr-xr-x   0        0        0      209 2020-02-02 00:00:00.000000 arm_jupyter_kernel-1.0.8/README.md
--rwxr-xr-x   0        0        0      451 2020-02-02 00:00:00.000000 arm_jupyter_kernel-1.0.8/hatch_build.py
--rwxr-xr-x   0        0        0     1761 2020-02-02 00:00:00.000000 arm_jupyter_kernel-1.0.8/pyproject.toml
--rw-r--r--   0        0        0    41892 2020-02-02 00:00:00.000000 arm_jupyter_kernel-1.0.8/PKG-INFO
+-rwxr-xr-x   0        0        0       89 2020-02-02 00:00:00.000000 arm_jupyter_kernel-1.1.0/arm_kernel/__init__.py
+-rwxr-xr-x   0        0        0      123 2020-02-02 00:00:00.000000 arm_jupyter_kernel-1.1.0/arm_kernel/__main__.py
+-rwxr-xr-x   0        0        0     3395 2020-02-02 00:00:00.000000 arm_jupyter_kernel-1.1.0/arm_kernel/arm_kernel.py
+-rwxr-xr-x   0        0        0       17 2020-02-02 00:00:00.000000 arm_jupyter_kernel-1.1.0/arm_kernel/const.py
+-rwxr-xr-x   0        0        0     6678 2020-02-02 00:00:00.000000 arm_jupyter_kernel-1.1.0/arm_kernel/emulator.py
+-rwxr-xr-x   0        0        0     2044 2020-02-02 00:00:00.000000 arm_jupyter_kernel-1.1.0/arm_kernel/install.py
+-rwxr-xr-x   0        0        0       96 2020-02-02 00:00:00.000000 arm_jupyter_kernel-1.1.0/arm_kernel/kernel.json
+-rwxr-xr-x   0        0        0    11666 2020-02-02 00:00:00.000000 arm_jupyter_kernel-1.1.0/arm_kernel/memory.py
+-rwxr-xr-x   0        0        0     5928 2020-02-02 00:00:00.000000 arm_jupyter_kernel-1.1.0/arm_kernel/preprocessor.py
+-rwxr-xr-x   0        0        0     9004 2020-02-02 00:00:00.000000 arm_jupyter_kernel-1.1.0/arm_kernel/registers.py
+-rwxr-xr-x   0        0        0     7545 2020-02-02 00:00:00.000000 arm_jupyter_kernel-1.1.0/arm_kernel/view.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 arm_jupyter_kernel-1.1.0/arm_kernel/templates/__init__.py
+-rwxr-xr-x   0        0        0      465 2020-02-02 00:00:00.000000 arm_jupyter_kernel-1.1.0/arm_kernel/templates/disassembly.py
+-rwxr-xr-x   0        0        0      352 2020-02-02 00:00:00.000000 arm_jupyter_kernel-1.1.0/arm_kernel/templates/memory.py
+-rwxr-xr-x   0        0        0      769 2020-02-02 00:00:00.000000 arm_jupyter_kernel-1.1.0/arm_kernel/templates/register.py
+-rwxr-xr-x   0        0        0      601 2020-02-02 00:00:00.000000 arm_jupyter_kernel-1.1.0/arm_kernel/templates/stack.py
+-rwxr-xr-x   0        0        0      244 2020-02-02 00:00:00.000000 arm_jupyter_kernel-1.1.0/.gitignore
+-rwxr-xr-x   0        0        0    35821 2020-02-02 00:00:00.000000 arm_jupyter_kernel-1.1.0/LICENSE
+-rwxr-xr-x   0        0        0      209 2020-02-02 00:00:00.000000 arm_jupyter_kernel-1.1.0/README.md
+-rwxr-xr-x   0        0        0      451 2020-02-02 00:00:00.000000 arm_jupyter_kernel-1.1.0/hatch_build.py
+-rwxr-xr-x   0        0        0     2083 2020-02-02 00:00:00.000000 arm_jupyter_kernel-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0    41916 2020-02-02 00:00:00.000000 arm_jupyter_kernel-1.1.0/PKG-INFO
```

### Comparing `arm_jupyter_kernel-1.0.8/arm_kernel/arm_kernel.py` & `arm_jupyter_kernel-1.1.0/arm_kernel/arm_kernel.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,16 +17,14 @@
         'name': 'Any text',
         'mimetype': 'text/html',
         'file_extension': '.txt',
     }
     banner = "ARM Assembly - code an ARM CPU"
     
     view = View()
-
-    
     
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
         self.emulator = Emulator()
 
     def _execute_code(self, content: dict):
         
@@ -51,29 +49,40 @@
                 self.emulator.add_memory_item(item)
 
         stream_content = {
             'metadata': {},
             'data': {'text/html': f"<p>-- kernel configured successfully --</p>"}
             }
         self.send_response(self.iopub_socket, 'display_data', stream_content)
-        
+    
+    def _handle_subroutine(self, subroutine: dict):
+        label = subroutine["label"]
+        self.emulator.add_subroutine(label, subroutine["code"])
+        stream_content = {
+            'metadata': {},
+            'data': {'text/html': f"<p>-- subroutine {label} registered successfully --</p>"}
+            }
+        self.send_response(self.iopub_socket, 'display_data', stream_content)
+
 
     def do_execute(self, code, silent, store_history=True, user_expressions=None, allow_stdin=False):
         if silent:
             return
 
         try:
             # Preprocess
             parsed_block = Preprocessor.parse(code)
             
             match parsed_block[0]:
                 case BlockType.TEXT:
                     self._execute_code(parsed_block[1])
                 case BlockType.CONFIG:
                     self._handle_config(parsed_block[1])
+                case BlockType.SUBROUTINE:
+                    self._handle_subroutine(parsed_block[1])
 
         except Exception as e:
                 self.report_error(e)
 
         return {'status': 'ok',
                 # The base class increments the execution count
                 'execution_count': self.execution_count,
```

### Comparing `arm_jupyter_kernel-1.0.8/arm_kernel/emulator.py` & `arm_jupyter_kernel-1.1.0/arm_kernel/emulator.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,53 +1,46 @@
 from __future__ import print_function
 from collections import OrderedDict
 from keystone import *
 from unicorn import *
 from unicorn.arm_const import *
+from capstone import *
 from collections import namedtuple
 import threading
 from fnmatch import fnmatch
 import re
 import pynumparser
 
-from arm_kernel.memory import Memory, MemoryItem
+from arm_kernel.memory import ItemType, Memory, MemoryItem, MemoryType
 from arm_kernel import registers
 
-
-
 # callback for tracing basic blocks
 def hook_block(uc, address, size, user_data):
     print(">>> Tracing basic block at 0x%x, block size = 0x%x" %(address, size))
 
 # callback for tracing instructions
 def hook_code(uc, address, size, user_data):
     print(">>> Tracing instruction at 0x%x, instruction size = 0x%x" %(address, size))
 
-def extract_cpu_state(uc):
-    # Dictionary to hold registers.
-    registers = OrderedDict()
 
-    for register in range(13):
-        registers["r%d" % register] = uc.reg_read(UC_ARM_REG_R0 + register)
-
-    registers["r13"] = uc.reg_read(UC_ARM_REG_SP)
-    registers["r14"] = uc.reg_read(UC_ARM_REG_LR)
-    
-    return {"registers": registers} 
+EmulatorState = namedtuple("EmulatorState", ("registers", "memory", "analysis"))
 
-EmulatorState = namedtuple("EmulatorState", ("registers", "memory"))
+TraceLine = namedtuple("TraceLine", ("address", "bytes", "mnemonic", "op_str"))
     
 class Emulator:
     
     def __init__(self):
 
         # Initialize emulation suite.
         self.asm = Ks(KS_ARCH_ARM, KS_MODE_ARM)
         self.emu = Uc(UC_ARCH_ARM, UC_MODE_ARM)
+        self.cs = Cs(CS_ARCH_ARM, CS_MODE_ARM)
         self.mem = Memory(self.emu)
+        
+        self.last_code = ""
 
         # Setup symbol resolution using managed memory.
         def sym_resolver(symbol, value):
             print("symbol: %s" % symbol.decode('utf-8'))
             address, _ = self.mem.find_item(symbol.decode('utf-8'))
             if address is not None:
                 value[0] = address
@@ -55,15 +48,15 @@
             
             return False 
 
         self.asm.sym_resolver = sym_resolver
 
         # Setup hooks:
         # tracing one instruction with customized callback
-        self.emu.hook_add(UC_HOOK_CODE, hook_code, begin=self.mem.codepad_address)
+        # self.emu.hook_add(UC_HOOK_CODE, hook_code, begin=self.mem.codepad_address)
 
         # Setup registers.
         self.registers = registers.get_registers(self.emu)
         
         # Set registers to 0
         for register in self.select_registers(['0-12']):
             register.val = 0
@@ -91,21 +84,38 @@
                 more = [
                     r for r in self.registers if r not in selected and fnmatch(r.name, g)
                 ]
                 selected += more
 
         return selected
 
+    def assemble(self, code:str, addrs:int = 0) -> tuple[bytes | list, int, Exception | None]:
+        try:
+            instrs, count = self.asm.asm(code, addrs, as_bytes=True)
+            return (instrs, count, None)
+        except Exception as e:
+            instrs, count, err = None, None, e
+            return (instrs, count, err)
+        
+    def disassemble(self, code: bytearray | bytes | list, addrs: int = 0, count: int = 0) -> tuple[str, any]:
+        res = ""
+        disasm = self.cs.disasm(code, offset=addrs, count=count)
+        rows = []
+        for i in disasm:
+            res += "0x%x:\t%s\t%s\t%s\n" % (i.address, i.bytes.hex(), i.mnemonic, i.op_str)
+            rows.append(i)
+        return (res, rows)
+
     def execute_code(self, code):
         ret = []  # ret == [instrs, None] or [None, error]
 
         def parse_assembly():
             err = None
             try:
-                instrs, count = self.asm.asm(code, as_bytes=True)
+                instrs, count = self.asm.asm(code, addr=self.mem.codepad_address, as_bytes=True)
                 ret.extend((instrs, count, None))
             except Exception as e:
                 instrs, count, err = None, None, e
                 ret.extend((instrs, count, err))
             
 
         th = threading.Thread(target=parse_assembly, daemon=True)
@@ -120,25 +130,61 @@
 
         # keystone failed?
         if err is not None:
             raise err
 
         # valid assembly but not instructions there (like a comment)
         if not assembled:
-            return EmulatorState(self.registers, self.mem)
+            return EmulatorState(self.registers, self.mem, {})
+        
+        # Disassemble for disassembly view
+        try:
+            res, disasm = self.disassemble(assembled, addrs=self.mem.codepad_address, count=count)
+
+        except CsError as e:
+            raise Exception("Error disassembling")
 
         try:
             # write machine code to be emulated to memory
             self.mem.write_code(assembled)  
 
             # emulate machine code
             until = self.mem.codepad_address + len(assembled)
             self.emu.ctl_remove_cache(self.mem.codepad_address, until+1)
-            self.emu.emu_start(self.mem.codepad_address, self.mem.codepad_address + len(assembled), timeout=5000000)
+            self.emu.emu_start(self.mem.codepad_address, until, timeout=5000000)
 
-            return EmulatorState(self.registers, self.mem)
+            self.last_code = code
+
+            analysis = {
+                "disassembly": disasm,
+                "disassembly_str": res
+            }
+            return EmulatorState(self.registers, self.mem, analysis)
 
         except UcError as e:
             raise Exception("Error executing: %s" % e)
     
     def add_memory_item(self, item: MemoryItem):
-        self.mem.add_item(item)
+        self.mem.add_item(item)
+        try:
+            self._init_ldr(item.label)
+        except:
+            pass
+
+    def add_subroutine(self, label, subroutine):
+        """Assembles and adds a subroutine to the subroutine memory region."""
+        subroutine_addrs = self.mem.subroutine_region.start
+        encoded, count, err = self.assemble(subroutine, subroutine_addrs)
+        if err is not None:
+            raise Exception(f"Error assembling subroutine: {err}")
+        item = MemoryItem(label, ItemType.RAW, MemoryType.SUBROUTINE, content=encoded)
+        return self.add_memory_item(item)
+
+    def _init_ldr(self, label: str):
+        """This resolves first LDR unicorn bug."""
+        # Memorize current r0 value to restore later.
+        r0_val = self.emu.reg_read(UC_ARM_REG_R0)
+        # Execute dummy LDR code.
+        code = f"""LDR R0, ={label}"""
+        self.execute_code(code)
+        # Restore original r0 value.
+        self.emu.reg_write(UC_ARM_REG_R0, r0_val)
```

### Comparing `arm_jupyter_kernel-1.0.8/arm_kernel/install.py` & `arm_jupyter_kernel-1.1.0/arm_kernel/install.py`

 * *Files identical despite different names*

### Comparing `arm_jupyter_kernel-1.0.8/arm_kernel/memory.py` & `arm_jupyter_kernel-1.1.0/arm_kernel/memory.py`

 * *Files 25% similar despite different names*

```diff
@@ -7,41 +7,45 @@
 
 # Sources:
 # - Memory class from bad-address/iasm
 # - https://docs.python.org/3/library/stdtypes.html
 
 from collections import namedtuple
 from enum import Enum
+import math
 from struct import pack
 from sortedcontainers import SortedList
 from unicorn import *
 from unicorn.arm_const import *
 
+from arm_kernel.const import KB_SIZE
+
 ALIGNMENT = 4 * 1024
 
 def next_aligned(n: int, alignment: int = ALIGNMENT) -> int:
     return (n + alignment) & -(alignment-1)
 
 STACK_ADDR = 0x0
-STACK_SZ = 1024*1024
+STACK_SZ = 4 * KB_SIZE
 
 # Default profile
-DEFAULT_BASE = 0x400000
-DEFAULT_CODEPAD_MEM_START = DEFAULT_BASE
-DEFAULT_CODEPAD_MEM_SZ = 500 * (1 << 10) #500kb
-DEFAULT_SUBROUTINE_MEM_START = next_aligned(DEFAULT_CODEPAD_MEM_START + DEFAULT_CODEPAD_MEM_SZ)
+DEFAULT_BASE = 0x4000
+
+DEFAULT_SUBROUTINE_MEM_START = DEFAULT_BASE
 DEFAULT_SUBROUTINE_MEM_SZ = 1 << 20 #1Mb
-DEFAULT_MAIN_MEM_START = next_aligned(DEFAULT_SUBROUTINE_MEM_START + DEFAULT_SUBROUTINE_MEM_SZ)
-DEFAULT_MAIN_MEM_SZ = 4 * (1 << 20) #4Mb
-DEFAULT_PAGE_SZ = 1 << 10 #1Kb
 
-DEFAULT_RW_MEM_START = DEFAULT_MAIN_MEM_START
-DEFAULT_RW_MEM_SZ = DEFAULT_PAGE_SZ
+DEFAULT_RW_MEM_START = next_aligned(DEFAULT_SUBROUTINE_MEM_START + DEFAULT_SUBROUTINE_MEM_SZ)
+DEFAULT_RW_MEM_SZ = 2 * (1 << 20) #2Mb
 DEFAULT_RO_MEM_START =  next_aligned(DEFAULT_RW_MEM_START + DEFAULT_RW_MEM_SZ)
-DEFAULT_RO_MEM_SZ = DEFAULT_PAGE_SZ
+DEFAULT_RO_MEM_SZ = 2 * (1 << 20) #2Mb
+
+DEFAULT_CODEPAD_MEM_START = next_aligned(DEFAULT_RO_MEM_START + DEFAULT_RO_MEM_SZ)
+DEFAULT_CODEPAD_MEM_SZ = 500 * (1 << 10) #500kb
+
+DEFAULT_PAGE_SZ = 1 << 10 #1Kb
 
 class MemoryType(Enum):
     CODE = 1
     MAIN = 2
     RO = 3
     RW = 4
     SUBROUTINE = 5 
@@ -49,23 +53,25 @@
 
 class ItemType(Enum):
     BYTE = 1
     HWORD = 2
     WORD = 4
     INT = 10
     STRING = 20
+    RAW = 21
     SPACE = 0
 
 ITEM_BYTE_SZ = {
     ItemType.BYTE: 1,
     ItemType.HWORD: 2,
     ItemType.WORD: 4,
     ItemType.INT: 4,
     ItemType.STRING: 1,
-    ItemType.SPACE: 1
+    ItemType.SPACE: 1,
+    ItemType.RAW: 1,
 }
 
 # Item: Tuple("label", type, access, size, content)
 class MemoryItem:
 
     def __init__(self, label: str, type: ItemType, access: MemoryType, size: int = 1, content = None):
         self.label = label
@@ -77,16 +83,19 @@
 
     def _type_bytes(self, type: ItemType) -> int:
         return ITEM_BYTE_SZ[type]
 
     def calculate_bytes_count(self):
         byte_count = self._type_bytes(self.type)
 
+        if self.type is ItemType.RAW:
+            return len(self.content)
+
         # Handle strings
-        if self.type is ItemType.STRING:
+        elif self.type is ItemType.STRING:
             if isinstance(self.content, list):
                 raise ValueError("Only strings must be single, not lists.")
             return len(self.content) + 1 # null terminate
             
         # Handle SPACE
         elif self.type is ItemType.SPACE:
             return self.size * self.byte_count
@@ -97,55 +106,36 @@
         else:
             return byte_count
 
     # ref: [https://www.geeksforgeeks.org/how-to-convert-int-to-bytes-in-python/]    
     def to_bytes(self):
         bytes_per_val = self._type_bytes(self.type)
 
+        if self.type is ItemType.RAW:
+            return self.content
+
         # Handle space
-        if self.type is ItemType.SPACE:
+        elif self.type is ItemType.SPACE:
             return bytes([0] * bytes_per_val * self.size)
         # Handle strings
         elif self.type is ItemType.STRING:
             if isinstance(self.content, list):
                 raise ValueError("Only single strings are supported.")
             return bytes(self.content, 'ascii') + b'\x00'
 
         # Handle list
-        if isinstance(self.content, list):
+        elif isinstance(self.content, list):
             byte_ls = []
             for val in self.content:
                 words = val.to_bytes(bytes_per_val, 'little')
                 for byte in words:
                     byte_ls.append(byte)
             return bytes(byte_ls)
         else:
             return self.content.to_bytes(bytes_per_val, 'little')
-    
-    def initialize(self, init):
-        for i in init:
-            if i['type'] == 'memory_i32':
-                # %s replaced with number of integers expected                
-                # # < means little-endian                
-                data = pack('<%si' % len(i['data']), *i['data'])
-                # assumes address in JSON is in hexadecimal string form                
-                self._mu.mem_write(int(i['address'], 16), data)
-            elif i['type'] == 'memory_i8':
-                # %s replaced with number of integers expected                
-                # < means little-endian                
-                data = pack('<%sb' % len(i['data']), *i['data'])
-                # assumes address in JSON is in hexadecimal string form                s
-                self._mu.mem_write(int(i['address'], 16), data)
-            elif i['type'] == 'memory_string':
-                # %s replaced with number of integers expected                
-                # < means little-endian               
-                data = bytes(i['string'], 'ascii') + b'\x00'                
-                # assumes address in JSON is in hexadecimal string form                
-                self._mu.mem_write(int(i['address'], 16), data)
-
 
 class MemoryPage:
 
     def __init__(self, type: MemoryType, start: int, capacity: int):
         self.type = type
         self.start = start
         self.capacity = capacity
@@ -169,106 +159,165 @@
         mu.mem_write(self.next_address, item.to_bytes())
         self.labels.append((item.label, self.next_address))
         
         self.next_address = next_aligned(self.next_address + item.byte_size, 4)
         if self.next_address >= self.start + self.capacity:
             self.is_full = True
         self.size = min(self.capacity, self.next_address - self.start)
+
+class MemoryRegion:
+    """Defines a functional memory unit (should be reserved for a specific purpose)"""
+
+    def __init__(self, mu: unicorn.Uc, start: int, end: int):
+         self.start = start
+         self.end = end
+         self._pages = SortedList(iterable=[], key=lambda x: x.start)
+         self._next_page_address = start
+         self._mu = mu
+         self._items = {}
+
+
+    def add_page(self, size: int = ALIGNMENT, type: MemoryType = MemoryType.RW) -> MemoryPage:
+        if  self._next_page_address + size - 1 > self.end:
+            raise ValueError(f"A page of size {size}b does not fit in this region")
+        
+        match(type):
+            case (MemoryType.RW | MemoryType.STACK):
+                perms = UC_PROT_ALL
+            case MemoryType.RO:
+                perms = UC_PROT_READ
+            case (MemoryType.CODE | MemoryType.SUBROUTINE):
+                perms = UC_PROT_EXEC | UC_PROT_READ
+            case _:
+                raise ValueError("Invalid memory type")
+        
+        # Map memory in Unicorn
+        try:
+            start = self._next_page_address
+            self._mu.mem_map(address=start, size=size, perms=perms)
+            self._memset(start, start + size - 1)
+        except Exception as e:
+            raise Exception(f"Error mapping memory in unicorn: {str(e)}")
+        
+        page = MemoryPage(type, self._next_page_address, size)
+        self._pages.add(page)
+        
+        # Update next address
+        self._next_page_address = next_aligned(self._next_page_address + size)
+        return page
+
+    def find_free_page(self, type: MemoryType, size: int, create: bool = True) -> MemoryPage:
+        for page in self._pages:
+            if page.type is type and page.capacity - page.size >= size:
+                return page
+        if create:
+            try:
+                page = self.add_page(ALIGNMENT * math.ceil(size/ALIGNMENT), type)
+                return page
+            except Exception as e:
+                raise Exception(f"No page with requested size found and page could not be created: {str(e)}.")
+        raise Exception(f"No page can be found with the requested size.")
+    
+    def add_item(self, item: MemoryItem):
+        # get page with space
+        page = self.find_free_page(item.access, item.byte_size)
+
+        # Add content to memory
+        addrs = page.next_address
+        try:
+            page.add_item(self._mu, item)
+        except Exception as error:
+            raise Exception(f"Error writing content to memory: {str(error)}")
+        else:
+            self._items[item.label] = (addrs, item.byte_size)
+    
+        return (addrs, item.byte_size)
+    
+    def find_item(self, label:str) -> tuple[int, int] | None:
+        return self._items.get(label)
+
+    def _memset(self, start, end, val: int = 0):
+        step = 0x2000  # 8k
+        if val:
+            data = bytes([val]) * step
+        else:
+            data = bytes(step)  # null initialized
+        for addr in range(start, end + 1, step):
+            if addr + step > end + 1:
+                data = data[:end - addr + 1]
+            self._mu.mem_write(addr, data)
+
+#= namedtuple("MemoryRegion", ("start", "end"))
         
 class Memory:
     def __init__(self, mu: unicorn.Uc):
         self._mu = mu
 
         # Setup main memory regions map
         self._mem_regions = {
-            MemoryType.STACK: (STACK_ADDR, STACK_ADDR + STACK_SZ - 1),
-            MemoryType.CODE: (DEFAULT_CODEPAD_MEM_START, DEFAULT_CODEPAD_MEM_START + DEFAULT_CODEPAD_MEM_SZ - 1), 
-            MemoryType.SUBROUTINE: (DEFAULT_SUBROUTINE_MEM_START, DEFAULT_SUBROUTINE_MEM_START + DEFAULT_SUBROUTINE_MEM_SZ - 1),
-            MemoryType.MAIN: (DEFAULT_MAIN_MEM_START, DEFAULT_MAIN_MEM_START +  DEFAULT_MAIN_MEM_SZ - 1)
+            MemoryType.STACK: MemoryRegion(self._mu, STACK_ADDR, STACK_ADDR + STACK_SZ - 1),
+            MemoryType.CODE: MemoryRegion(self._mu, DEFAULT_CODEPAD_MEM_START, DEFAULT_CODEPAD_MEM_START + DEFAULT_CODEPAD_MEM_SZ - 1), 
+            MemoryType.SUBROUTINE: MemoryRegion(self._mu, DEFAULT_SUBROUTINE_MEM_START, DEFAULT_SUBROUTINE_MEM_START + DEFAULT_SUBROUTINE_MEM_SZ - 1),
+            MemoryType.RW: MemoryRegion(self._mu, DEFAULT_RW_MEM_START, DEFAULT_RW_MEM_START +  DEFAULT_RW_MEM_SZ - 1),
+            MemoryType.RO: MemoryRegion(self._mu, DEFAULT_RO_MEM_START, DEFAULT_RO_MEM_START +  DEFAULT_RO_MEM_SZ - 1),
         }
-
-        self._mu.mem_map(address=DEFAULT_CODEPAD_MEM_START, size=DEFAULT_CODEPAD_MEM_SZ, perms=UC_PROT_EXEC | UC_PROT_READ)
-        self._memset(self._mem_regions[MemoryType.CODE])
-        self._mu.mem_map(address=DEFAULT_SUBROUTINE_MEM_START, size=DEFAULT_SUBROUTINE_MEM_SZ, perms=UC_PROT_EXEC | UC_PROT_READ)
-        self._memset(self._mem_regions[MemoryType.SUBROUTINE])
+        
+        # Configure codepad region
+        self._mem_regions[MemoryType.CODE].add_page(DEFAULT_CODEPAD_MEM_SZ, MemoryType.CODE)
+        
+        # Configure subroutine region.
+        self._mem_regions[MemoryType.SUBROUTINE].add_page(DEFAULT_SUBROUTINE_MEM_SZ, MemoryType.SUBROUTINE)
+        
         # Configure stack
-        self._mu.mem_map(address=STACK_ADDR, size=STACK_SZ)
-        self._memset(self._mem_regions[MemoryType.STACK])
+        self._mem_regions[MemoryType.STACK].add_page(STACK_SZ, MemoryType.STACK)
         self._mu.reg_write(UC_ARM_REG_SP, STACK_ADDR + STACK_SZ)
         self._mu.reg_write(UC_ARM_REG_FP, STACK_ADDR + STACK_SZ)
 
-        # Setup pages map
-        self._rw_pages = SortedList(iterable=[
-            MemoryPage(MemoryType.RW, DEFAULT_RW_MEM_START, DEFAULT_RW_MEM_SZ)
-        ], key=lambda x: x.start)
-
-        self._ro_pages = SortedList(iterable=[
-            MemoryPage(MemoryType.RO, DEFAULT_RO_MEM_START, DEFAULT_RO_MEM_SZ)
-        ], key=lambda x: x.start)
-
-        self._mu.mem_map(DEFAULT_RW_MEM_START, DEFAULT_RW_MEM_SZ)
-        self._memset((DEFAULT_RW_MEM_START, DEFAULT_RW_MEM_START + DEFAULT_RW_MEM_SZ - 1))
-        self._mu.mem_map(DEFAULT_RO_MEM_START, DEFAULT_RO_MEM_SZ, perms=UC_PROT_READ)
-        self._memset((DEFAULT_RO_MEM_START, DEFAULT_RO_MEM_START + DEFAULT_RO_MEM_SZ - 1))
+        # Setup main memory
+        self._mem_regions[MemoryType.RO].add_page(type=MemoryType.RO)
+        self._mem_regions[MemoryType.RW].add_page(type=MemoryType.RW)
 
+        # Initialize items dict
         self._items = {}
 
+
     @property
     def codepad_address(self) -> int:
-        return self._mem_regions[MemoryType.CODE][0]
+        return self._mem_regions[MemoryType.CODE].start
 
     @property
     def stack_region(self) -> tuple[int, int]:
-        return self._mem_regions[MemoryType.STACK]
-
-    # ref: mem.py in https://book-of-gehn.github.io/articles/2021/01/09/Interactive-Assembler.html
-    def _memset(self, region: tuple[int, int], val: int = 0):
-        step = 0x2000  # 8k
-        if val:
-            data = bytes([val]) * step
-        else:
-            data = bytes(step)  # null initialized
-        for addr in range(region[0], region[1] + 1, step):
-            if addr + step > region[1] + 1:
-                data = data[:region[1] - addr + 1]
-            self._mu.mem_write(addr, data)
+        stack_region = self._mem_regions[MemoryType.STACK]
+        return (stack_region.start, stack_region.end)
+    
+    @property
+    def subroutine_region(self) -> MemoryRegion:
+        return self._mem_regions[MemoryType.SUBROUTINE]
 
-    def _find_page(self, access: MemoryType, size: int) -> MemoryPage:
-        # Find memory list
-        list = SortedList()
-        if access is MemoryType.RO:
-            list = self._ro_pages
-        else:
-            list = self._rw_pages
-        
-        for page in list:
-            if page.capacity - page.size >= size:
-                return page
-        
-        #TODO: Create new page if no page found
-        raise Exception("No page found") # this will be substituted by the creation of a new page
+    def _find_region(self, access: MemoryType, size: int) -> MemoryRegion:
+        return self._mem_regions[access]
 
     def write_code(self, code: bytes):
-        address = self._mem_regions[MemoryType.CODE][0]
+        address = self._mem_regions[MemoryType.CODE].start
         self._mu.mem_write(address, code)  
 
     def add_item(self, item: MemoryItem):
         #TODO: Validate item.
 
         # get page with space
-        page = self._find_page(item.access, item.byte_size)
+        region = self._find_region(item.access, item.byte_size)
 
         # Add content to memory
-        addrs = page.next_address
         try:
-            page.add_item(self._mu, item)
+            addrs = region.add_item(item)[0]
         except Exception as error:
             raise Exception(f"Error writing content to memory: {str(error)}")
         else:
             self._items[item.label] = (addrs, item.byte_size)
+            return (addrs, item.byte_size)
     
     def read_item(self, label: str) -> bytearray:
         item = self._items[label]
         print(item)
         content = self._mu.mem_read(item[0], item[1])
         return content
```

### Comparing `arm_jupyter_kernel-1.0.8/arm_kernel/preprocessor.py` & `arm_jupyter_kernel-1.1.0/arm_kernel/preprocessor.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 from enum import Enum
 import yaml
 from yaml.loader import SafeLoader
 from arm_kernel.memory import MemoryItem, MemoryType, ItemType
 import re
 
-CODE_1 = """__config__
+sample_config = """__config__
 memory:
     items:
         label1:
             type: word
             content: [1,2,3,4]
             access: ro
         label2:
             type: byte
             content: [1,2,3,4]
             access: rw
 """
-CODE_2 = """
-LDR R0, =test
-LDR R1, [R0]
-LDR R2, [R0, #8]
-MOV R0, R1
->>> show registers
+
+sample_subroutine = """__subroutine:upr__
+upr:
+    code...
 """
 
 show_re = re.compile(r"^>>>\s+show\s+(?P<view>[a-zA-Z]+)(\[(?P<context>[a-zA-Z0-9,\-:]*)\])?(\s+as\s+(?P<format>[a-z]+))?")
 decimal_imm_re = re.compile(r'(?:#|=)\d\d+(?![a-zA-Z])')
+subroutine_re = re.compile(r"__subroutine:(?P<label>\S+)__")
 
 class BlockType(Enum):
     INVALID = 0
     TEXT = 1
     CONFIG = 2
+    SUBROUTINE = 3
     MEM_FUNC = 4
 
 class Preprocessor:
 
     @staticmethod
     def parse(text: str) -> tuple:
         # remove whitespace from beginning of line.
@@ -48,28 +48,36 @@
         block_type = Preprocessor.parse_type(partition[0])
 
         content = {}
         match block_type:
             case BlockType.CONFIG:
                 content = Preprocessor.parse_config(partition[1])
             case BlockType.TEXT:
-                views, cleaned_code = Preprocessor.process_code(text)
+                views, code = Preprocessor.process_code(text)
                 content = {
-                    "code": cleaned_code,
+                    "code": code,
                     "views": views
                 }
+            case BlockType.SUBROUTINE:
+                label, code = Preprocessor.process_subroutine(text)
+                content = {
+                    "label": label,
+                    "code": code,
+                }
 
         return (
             block_type,
             content
         )
     
     @staticmethod
     def parse_type(line: str) -> BlockType:
         line = line.strip()
+        if subroutine_re.match(line) is not None:
+            return BlockType.SUBROUTINE
         match line:
             case "__config__":
                 return BlockType.CONFIG
             case _:
                 return BlockType.TEXT
 
     @staticmethod
@@ -163,9 +171,20 @@
             match = show_re.search(line)
             if match is not None:
                 views.append(match.groupdict())
             else:
                 cleaned_code.append(line)
         
         return views, '\n'.join(cleaned_code)
+    
+    @staticmethod
+    def process_subroutine(content: str) -> tuple[str, str]:
+        partition = content.split('\n', 1)
+        heading = partition[0]
+        code = partition[1]
+        heading_match = subroutine_re.match(heading)
+        label = heading_match.groupdict()["label"]
+        _, cleaned_code = Preprocessor.process_code(code)
+        return (label, cleaned_code)
+
```

### Comparing `arm_jupyter_kernel-1.0.8/arm_kernel/registers.py` & `arm_jupyter_kernel-1.1.0/arm_kernel/registers.py`

 * *Files identical despite different names*

### Comparing `arm_jupyter_kernel-1.0.8/arm_kernel/view.py` & `arm_jupyter_kernel-1.1.0/arm_kernel/view.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from fnmatch import fnmatch
 from jinja2 import Environment, FileSystemLoader
 import pynumparser
 
 from arm_kernel.templates.register import DETAILED_REGISTERS_TEMPLATE, NZCV_FLAGS_VIEW
 from arm_kernel.templates.stack import STACK_VIEW
 from arm_kernel.templates.memory import MEMORY_WORD_VIEW
+from arm_kernel.templates.disassembly import SIMPLE_DISASSEMBLY_VIEW
 from arm_kernel.emulator import EmulatorState
 from arm_kernel import registers
 from arm_kernel import memory
 
 re_single_label = re.compile(r'^\w+$')
 
 class View:
@@ -23,23 +24,25 @@
         self.env = Environment()
 
     def get_view(self, view_config: dict, state: EmulatorState) -> str:
         '''Get HTML content representing a view of the CPU state'''
 
         match view_config["view"]:
             case "registers":
-                return self.gen_registers_view(view_config, state)
+                return self.generate_registers_view(view_config, state)
             case "stack":
-                return self.gen_stack_view(view_config, state)
+                return self.generate_stack_view(view_config, state)
             case ("nzcv" | "flags"):
-                return self.gen_nzcv_flags_view(state)
+                return self.generate_nzcv_flags_view(state)
             case ("mem" | "memw" | "memh" | "memb") as mem_mode:
-                return self.gen_mem_view(view_config, state, mem_mode)
+                return self.generate_mem_view(view_config, state, mem_mode)
+            case ("disassembly" | "disasm"):
+                return self.generate_disassembly_view(view_config, state)
     
-    def gen_stack_view(self, view_config: dict, state: EmulatorState) -> str:
+    def generate_stack_view(self, view_config: dict, state: EmulatorState) -> str:
         template = self.env.from_string(STACK_VIEW)
         sp = self.select_registers(state.registers, ["sp"])[0]
         mem = state.memory
         sp_region = mem.stack_region
         rows = []
         for addrs in range(sp_region[1]-3, sp.val - 4, -4):
             print(hex(addrs))
@@ -50,15 +53,15 @@
         context = {
             "content": rows,
             "bottom_address": self._format(sp_region[1]+1, "hex"),
             "sp": self._format(sp.val, "hex")
         }
         return template.render(context)
 
-    def gen_mem_view(self, view_config: dict, state: EmulatorState, mem_mode: str = "memw") -> str:
+    def generate_mem_view(self, view_config: dict, state: EmulatorState, mem_mode: str = "memw") -> str:
         template = self.env.from_string(MEMORY_WORD_VIEW)
         mem = state.memory
 
         metadata, content_bytes = self._get_memory_from_context(mem, view_config['context'])
         content_bytes += bytes([0] * (len(content_bytes)%4))
         
         init_addrss = metadata[0]
@@ -90,40 +93,52 @@
         }
         return template.render(context)
         # return f"""
         # <p>{str(content_bytes)}</p>
         # <p>{str(rows)}</p>
         # """
 
-    def gen_nzcv_flags_view(self, state: EmulatorState) -> str:
+    def generate_nzcv_flags_view(self, state: EmulatorState) -> str:
         template = self.env.from_string(NZCV_FLAGS_VIEW)
         cpsr = self.select_registers(state.registers, ["cpsr"])[0]
         context = {
             "n": cpsr.N.fget().bin,
             "z": cpsr.Z.fget().bin,
             "c": cpsr.C.fget().bin,
             "v": cpsr.V.fget().bin
         }
         return template.render(context)
 
-    def gen_registers_view(self, view_config: dict, state: EmulatorState) -> str:
+    def generate_registers_view(self, view_config: dict, state: EmulatorState) -> str:
         template = self.env.from_string(DETAILED_REGISTERS_TEMPLATE)
         if "context" in view_config and view_config["context"] is not None:
             pattern = view_config["context"].split(",")
         else:
             pattern = ["0-12"]
         selected = self.select_registers(state.registers, pattern)
         registers = [(r.name, self._format(r.val, view_config.get("format"))) for r in selected]
         context = {
             "registers": registers,
             "reg_count": len(selected)
         }
-        print(context)
         return template.render(context)
 
+    def generate_disassembly_view(self, view_config: dict, state: EmulatorState) -> str:
+        template = self.env.from_string(SIMPLE_DISASSEMBLY_VIEW)
+        rows = []
+        for i in state.analysis["disassembly"]:
+            rows.append((self._padhexa(hex(i.address)), f"0x{i.bytes.hex()}", i.mnemonic, i.op_str))
+
+        context = {
+            "disassembly": rows,
+        }
+        return template.render(context)
+        
+
+
     def select_registers(self, registers, patterns) -> list[registers.Register]:
         '''Filter the registers by name following the globs expressions.'''
 
         parser = pynumparser.NumberSequence()
 
         if not patterns:
             return list()
@@ -170,15 +185,15 @@
             return r'\x{0:02x}'.format(c)
         elif c <= '\uffff':
             return r'\u{0:04x}'.format(c)
         else:
             return r'\U{0:08x}'.format(c)
 
     @staticmethod
-    def _padhexa(s: str, size: int):
+    def _padhexa(s: str, size: int = 8):
         return '0x' + s[2:].zfill(size)
 
     def _get_memory_from_context(self, mem: memory.Memory, context) -> tuple[tuple[int, int], bytearray]:
         if re_single_label.fullmatch(context) is None:
             raise Exception("Error: memory address pattern is not valid.")
         
         label = context
```

### Comparing `arm_jupyter_kernel-1.0.8/arm_kernel/templates/stack.py` & `arm_jupyter_kernel-1.1.0/arm_kernel/templates/stack.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 STACK_VIEW = """
 <h4>Stack:</h4>
-<table>
+<table style='font-family:"Courier New", Courier, monospace;'>
 <tr>
     <th>Address</th>
     <th>Content</th>
     <th>SP</th>
 </tr>
 <tr>
     <td>{{bottom_address}}</td>
```

### Comparing `arm_jupyter_kernel-1.0.8/LICENSE` & `arm_jupyter_kernel-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `arm_jupyter_kernel-1.0.8/pyproject.toml` & `arm_jupyter_kernel-1.1.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -7,14 +7,15 @@
   "Jinja2>=3.1.2",
   "keystone_engine>=0.9.2",
   "pynumparser>=1.4.1",
   "pyparsing>=3.0.9",
   "PyYAML>=6.0",
   "sortedcontainers>=2.4.0",
   "unicorn",
+  "capstone",
   "cmake",
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "arm-jupyter-kernel"
 description = 'Jupyter kernel for ARM Assemble language.'
@@ -40,14 +41,15 @@
   "Jinja2>=3.1.2",
   "keystone_engine>=0.9.2",
   "pynumparser>=1.4.1",
   "pyparsing>=3.0.9",
   "PyYAML>=6.0",
   "sortedcontainers>=2.4.0",
   "unicorn==2.0.1.post1",
+  "capstone",
 ]
 dynamic = ["version"]
 
 [project.urls]
 Documentation = "https://github.com/SamuelAl/arm_kernel#readme"
 Issues = "https://github.com/SamuelAl/arm_kernel/issues"
 Source = "https://github.com/SamuelAl/arm_kernel"
@@ -58,14 +60,23 @@
 # Used to call hatch_build.py
 [tool.hatch.build.hooks.custom]
 
 [tool.pytest.ini_options]
 pythonpath = [
   "."
 ]
+filterwarnings = [
+    "error",
+    "ignore::UserWarning",
+    "ignore::DeprecationWarning:unicorn",
+    "ignore::DeprecationWarning:jupyter",
+    # note the use of single quote below to denote "raw" strings in TOML
+    'ignore:function ham\(\) is deprecated:DeprecationWarning',
+]
+
 
 [tool.hatch.build.targets.sdist]
 include = [
     "/arm_kernel",
 ]
 
 [tool.hatch.build.targets.wheel.shared-data]
```

### Comparing `arm_jupyter_kernel-1.0.8/PKG-INFO` & `arm_jupyter_kernel-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arm-jupyter-kernel
-Version: 1.0.8
+Version: 1.1.0
 Summary: Jupyter kernel for ARM Assemble language.
 Project-URL: Documentation, https://github.com/SamuelAl/arm_kernel#readme
 Project-URL: Issues, https://github.com/SamuelAl/arm_kernel/issues
 Project-URL: Source, https://github.com/SamuelAl/arm_kernel
 Author-email: "Alarco Cantos, Samuel" <alarcocs@tcd.ie>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
@@ -686,14 +686,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
 Requires-Dist: bitstring>=4.0.1
+Requires-Dist: capstone
 Requires-Dist: ipykernel>=6.20.2
 Requires-Dist: jinja2>=3.1.2
 Requires-Dist: jupyter-client
 Requires-Dist: keystone-engine>=0.9.2
 Requires-Dist: pynumparser>=1.4.1
 Requires-Dist: pyparsing>=3.0.9
 Requires-Dist: pyyaml>=6.0
```

