# RT-Thread building script for trace component

from building import *

src_folder = 'SystemView_Src'

cwd = GetCurrentDir()
src = Glob(src_folder +'/Config/*.c')
src += Glob(src_folder +'/SEGGER/*.c')

CPPPATH = [cwd, os.path.join(cwd, src_folder+'/Config')]
CPPPATH += [cwd, os.path.join(cwd, src_folder+'/SEGGER')]
group = DefineGroup('trace', src, depend = ['PKG_USING_SYSTEMVIEW'], CPPPATH = CPPPATH)

Return('group')
