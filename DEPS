vars = {
  'chromium_git': 'https://chromium.googlesource.com'
}

deps = { 
  'src/buildtools':
    (Var("chromium_git")) + '/external/github.com/google/open-vcdiff.git@21d7d0b9c3d0c3ccbdb221c85ae889373f0a2a58',
  'src/testing/gmock':
    (Var("chromium_git")) + '/external/googlemock.git@0421b6f358139f02e102c9c332ce19a33faf75be',
  'src/testing/gtest':
    (Var("chromium_git")) + '/external/github.com/google/googletest.git@6f8a66431cb592dad629028a50b3dd418a408c87',
  'src/third_party/icu':
    (Var("chromium_git")) + '/chromium/deps/icu.git@8f91ea3a7e0413df3312204058da856058a8099b',
}

deps_os = { 
  'win': { 
  }
}

hooks = [
 
]

include_rules = [
  '+base',
  '+build'
]

skip_child_includes = [

]
