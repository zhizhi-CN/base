vars = {
  'chromium_git': 'https://chromium.googlesource.com'
}

deps = { 
  'src/breakpad/src':
    (Var("chromium_git")) + '/breakpad/breakpad/src.git@ba0a8cb51c79845955cd0f262fe1a2a5f1ead9b9',
  'src/buildtools':
    (Var("chromium_git")) + '/chromium/buildtools.git@0f8e6e4b126ee88137930a0ae4776c4741808740',
  'src/tools/gyp':
    (Var("chromium_git")) + '/external/gyp.git@54b7dfc03f746b6a539ac38f2fb0815d10b54734',
  'src/testing/gmock':
    (Var("chromium_git")) + '/external/googlemock.git@0421b6f358139f02e102c9c332ce19a33faf75be',
  'src/testing/gtest':
    (Var("chromium_git")) + '/external/github.com/google/googletest.git@6f8a66431cb592dad629028a50b3dd418a408c87',
  'src/third_party/icu':
    (Var("chromium_git")) + '/chromium/deps/icu.git@8f91ea3a7e0413df3312204058da856058a8099b',
  'src/third_party/boringssl/src':
    'https://boringssl.googlesource.com/boringssl.git@907ae62b9d81121cb86b604f83e6b811a43f7a87',
  'src/third_party/yasm/source/patched-yasm':
    (Var("chromium_git")) + '/chromium/deps/yasm/patched-yasm.git@4671120cd8558ce62ee8672ebf3eb6f5216f909b'
}

deps_os = { 
  'win': { 
  }
}

hooks = [
   {
    'action': [
      'download_from_google_storage',
      '--no_resume',
      '--platform=win32',
      '--no_auth',
      '--bucket',
      'chromium-gn',
      '-s',
      'src/buildtools/win/gn.exe.sha1'
    ],
    'pattern':
      '.',
    'name':
      'gn_win'
  }
]

include_rules = [
  '+base',
  '+build'
]

skip_child_includes = [

]
