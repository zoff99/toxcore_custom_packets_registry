# Tox - Custom Packets Registry

Tox Packet ID is a ```uint8_t``` <br>
the valid packet range is from ```0 ... 254``` <br>
(255 is not included, i do not know the reason for this) <br>

the packet ranges are defined here:
https://github.com/zoff99/c-toxcore/blob/zoff99/zoxcore_local_fork/toxcore/net_crypto.h#L23-L42

kind: <br>
```LS lossless``` <br>
```LY lossy``` <br>

### tabular form:

|Packet ID       |kind|used by                                    | link
|:---------------|:---|:------------------------------------------|:-------------
| [0..15]        | LS | reserved for net_crypto internal use      | https://github.com/zoff99/c-toxcore/blob/f5c2c56560011dba380f99fd7b895516d90a0df6/toxcore/net_crypto.h#L23-L42
| [16..159]      | LS | reserved for Messenger internal use       | https://github.com/zoff99/c-toxcore/blob/f5c2c56560011dba380f99fd7b895516d90a0df6/toxcore/net_crypto.h#L23-L42
| 160            | LS | ToxPhone                                  | https://github.com/hkarel/ToxPhone/blob/ce03405652b4ae80ef1dbc4b72b2b5048ec53668/src/toxphone/tox/tox_func.cpp#L131
| 161            | LS |                                           |
| 162            | LS |                                           |
| 163            | LS |                                           |
| 164            | LS |                                           |
| 165            | LS |                                           |
| 166            | LS |                                           |
| 167            | LS |                                           |
| 168            | LS |                                           |
| 169            | LS |                                           |
| 170            | LS | TRIfA, Zoxcore                            | https://github.com/zoff99/ToxAndroidRefImpl/blob/zoff99/dev003/jni-c-toxcore/jni-c-toxcore.c#L1029 <br> https://github.com/zoff99/c-toxcore/blob/f5c2c56560011dba380f99fd7b895516d90a0df6/toxutil/toxutil.c#L41
| 171            | LS |                                           |
| 172            | LS | ToxExt, TRIfA                             | https://github.com/toxext/toxext/blob/37449a144e0b03821f707c7847d595444956cc03/src/toxext.c#L10 <br> https://github.com/zoff99/c-toxcore/blob/f5c2c56560011dba380f99fd7b895516d90a0df6/toxav/rtp.c#L1260
| 173            | LS |                                           |
| 174            | LS | isotoxin                                  | https://github.com/isotoxin/isotoxin/blob/master/source/plugins/proto_tox/proto_tox.cpp#L88
| 175            | LS | TRIfA, ToxProxy, isotoxin                 | https://github.com/zoff99/ToxAndroidRefImpl/blob/zoff99/dev003/android-refimpl-app/app/src/main/java/com/zoffcc/applications/trifa/TRIFAGlobals.java#L221-L226 <br> https://github.com/kaefert/ToxProxy/blob/master/src/ToxProxy.c#L1404 <br> https://github.com/isotoxin/isotoxin/blob/master/source/plugins/proto_tox/proto_tox.cpp#L89
| 176            | LS | TRIfA, isotoxin                           | https://github.com/zoff99/ToxAndroidRefImpl/blob/zoff99/dev003/jni-c-toxcore/jni-c-toxcore.c#L1030 <br> https://github.com/isotoxin/isotoxin/blob/master/source/plugins/proto_tox/proto_tox.cpp#L90
| 177            | LS |                                           |
| 178            | LS |                                           |
| 179            | LS | TRIfA, ToxProxy                           | https://github.com/zoff99/ToxAndroidRefImpl/blob/zoff99/dev003/android-refimpl-app/app/src/main/java/com/zoffcc/applications/trifa/TRIFAGlobals.java#L221-L226 <br> https://github.com/kaefert/ToxProxy/blob/master/src/ToxProxy.c#L1394
| 180            | LS |                                           |
| 181            | LS | TRIfA                                     | https://github.com/zoff99/ToxAndroidRefImpl/blob/zoff99/dev003/jni-c-toxcore/jni-c-toxcore.c#L1031
| 182            | LS |                                           |
| 183            | LS |                                           |
| 184            | LS |                                           |
| 185            | LS |                                           |
| 186            | LS |                                           |
| 187            | LS |                                           |
| 188            | LS |                                           |
| 189            | LS |                                           |
| 190            | LS |                                           |
| 191            | LS |                                           |
| [192..199]     | LY | reserved for ToxAV internal use           | https://github.com/zoff99/c-toxcore/blob/f5c2c56560011dba380f99fd7b895516d90a0df6/toxcore/net_crypto.h#L23-L42
| 200            | LY |                                           |
| 201            | LY |                                           |
| 202            | LY |                                           |
| 203            | LY |                                           |
| 204            | LY |                                           |
| 205            | LY |                                           |
| 206            | LY |                                           |
| 207            | LY |                                           |
| 208            | LY |                                           |
| 209            | LY |                                           |
| 210            | LY |                                           |
| 211            | LY |                                           |
| 212            | LY |                                           |
| 213            | LY |                                           |
| 214            | LY |                                           |
| 215            | LY |                                           |
| 216            | LY |                                           |
| 217            | LY |                                           |
| 218            | LY |                                           |
| 219            | LY |                                           |
| 220            | LY |                                           |
| 221            | LY |                                           |
| 222            | LY |                                           |
| 223            | LY |                                           |
| 224            | LY |                                           |
| 225            | LY |                                           |
| 226            | LY |                                           |
| 227            | LY |                                           |
| 228            | LY |                                           |
| 229            | LY |                                           |
| 230            | LY |                                           |
| 231            | LY |                                           |
| 232            | LY |                                           |
| 233            | LY |                                           |
| 234            | LY |                                           |
| 235            | LY |                                           |
| 236            | LY |                                           |
| 237            | LY |                                           |
| 238            | LY |                                           |
| 239            | LY |                                           |
| 240            | LY |                                           |
| 241            | LY |                                           |
| 242            | LY |                                           |
| 243            | LY |                                           |
| 244            | LY |                                           |
| 245            | LY |                                           |
| 246            | LY |                                           |
| 247            | LY |                                           |
| 248            | LY |                                           |
| 249            | LY |                                           |
| 250            | LY |                                           |
| 251            | LY |                                           |
| 252            | LY |                                           |
| 253            | LY |                                           |
| 254            | LY |                                           |



### list form:

#### Zoxcore (ToxAV):

172 lossless
https://github.com/zoff99/c-toxcore/blob/zoff99/zoxcore_local_fork/toxav/rtp.c#L1260

PACKET_TOXAV_COMM_CHANNEL_FUNCTION: used for extended ToxAV commands
https://github.com/zoff99/c-toxcore/blob/zoff99/zoxcore_local_fork/toxav/video.h#L57-L63

#### c-toxcore ToxAV internal

69 lossless
https://github.com/zoff99/c-toxcore/blob/zoff99/zoxcore_local_fork/toxav/msi.c#L132

192 lossy
https://github.com/zoff99/c-toxcore/blob/zoff99/zoxcore_local_fork/toxav/rtp.c#L1257

193 lossy
https://github.com/zoff99/c-toxcore/blob/zoff99/zoxcore_local_fork/toxav/rtp.c#L1258

196 lossy
https://github.com/zoff99/c-toxcore/blob/zoff99/zoxcore_local_fork/toxav/bwcontroller.c#L294

#### Zoxcore (toxcore):

170 lossless
https://github.com/zoff99/c-toxcore/blob/zoff99/zoxcore_local_fork/toxutil/toxutil.c#L41

CAP_PACKET_ID: use to signal for toxutil extension

#### ToxExt:

172 lossless
https://github.com/toxext/toxext/blob/master/src/toxext.c#L10

TOXEXT_MAGIC: used as start byte of UUID to signal ToxExt extension

#### TRIfA (usually the same for TRIfA Desktop):

170 lossless
https://github.com/zoff99/ToxAndroidRefImpl/blob/zoff99/dev003/jni-c-toxcore/jni-c-toxcore.c#L1029

just forwarded to toxutil

175 lossless
https://github.com/zoff99/ToxAndroidRefImpl/blob/zoff99/dev003/android-refimpl-app/app/src/main/java/com/zoffcc/applications/trifa/TRIFAGlobals.java#L221-L226

176 lossless
https://github.com/zoff99/ToxAndroidRefImpl/blob/zoff99/dev003/jni-c-toxcore/jni-c-toxcore.c#L1030

179 lossless
https://github.com/zoff99/ToxAndroidRefImpl/blob/zoff99/dev003/android-refimpl-app/app/src/main/java/com/zoffcc/applications/trifa/TRIFAGlobals.java#L221-L226

181 lossless
https://github.com/zoff99/ToxAndroidRefImpl/blob/zoff99/dev003/jni-c-toxcore/jni-c-toxcore.c#L1031

#### ToxProxy

175 lossless
https://github.com/kaefert/ToxProxy/blob/master/src/ToxProxy.c#L1404

179 lossless
https://github.com/kaefert/ToxProxy/blob/master/src/ToxProxy.c#L1394

#### isotoxin

174 lossless
https://github.com/isotoxin/isotoxin/blob/master/source/plugins/proto_tox/proto_tox.cpp#L88

PACKETID_EXTENSION: used for commands and folder sharing

175 lossless
https://github.com/isotoxin/isotoxin/blob/master/source/plugins/proto_tox/proto_tox.cpp#L89

PACKETID_VIDEO_EX: used for custom video

176 lossless
https://github.com/isotoxin/isotoxin/blob/master/source/plugins/proto_tox/proto_tox.cpp#L90

PACKETID_AUDIO_EX: used for custom audio

