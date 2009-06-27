
require 'rake/clean'

sdk_location = '/Users/jan/projects/android-sdk-mac_x86-1.5_r1'
gen = 'gen'
res = 'res'
android_jar = "#{sdk_location}/platforms/android-1.5/android.jar"

directory gen

CLEAN.include(gen)

task :res_src => [gen]  do
  sh "aapt package -m -J #{gen} -M AndroidManifest.xml -S #{res} -I #{android_jar}"
end

#<echo>Compiling aidl files into Java classes...</echo>
#        <apply executable="${aidl}" failonerror="true">
#            <arg value="-p${android-aidl}" />
#            <arg value="-I${source-folder}" />
#            <arg value="-o${gen-folder}" />
#            <fileset dir="${source-folder}">
#                <include name="**/*.aidl"/>
#            </fileset>
#</apply>


