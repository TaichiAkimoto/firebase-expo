# firebase-expo
参考記事`https://rnfirebase.io/docs/v5.x.x/installation/android`

## コマンド
```
yarn
cd android
 ./gradlew clean
 ./gradlew installDevKernelDebug
```

## エラー
```

> Task :react-native-firebase:compileDebugRenderscript FAILED

FAILURE: Build failed with an exception.

* What went wrong:
Could not resolve all files for configuration ':react-native-firebase:debugCompileClasspath'.
> Could not resolve com.squareup.okhttp3:okhttp:3.10.0.
  Required by:
        project :react-native-firebase
	   > Cannot find a version of 'com.squareup.okhttp3:okhttp' that satisfies the version constraints:
	           Dependency path 'android:react-native-firebase:unspecified' --> 'com.facebook.react:react-native:32.0.0' --> 'com.squareup.okhttp3:okhttp:3.10.0'
		           Dependency path 'android:react-native-firebase:unspecified' --> 'com.google.firebase:firebase-functions:16.3.0' --> 'com.squareup.okhttp3:okhttp:3.12.1'
			           Dependency path 'android:react-native-firebase:unspecified' --> 'com.facebook.react:react-native:32.0.0' --> 'com.facebook.fresco:imagepipeline-okhttp3:1.10.0' --> 'com.squareup.okhttp3:okhttp:3.10.0'
				           Dependency path 'android:react-native-firebase:unspecified' --> 'com.facebook.react:react-native:32.0.0' --> 'com.squareup.okhttp3:okhttp-urlconnection:3.10.0' --> 'com.squareup.okhttp3:okhttp:3.10.0'
					           Constraint path 'android:react-native-firebase:unspecified' --> 'com.squareup.okhttp3:okhttp' strictly '3.10.0' because of the following reason: debugRuntimeClasspath uses version 3.10.0
						           Constraint path 'android:react-native-firebase:unspecified' --> 'com.squareup.okhttp3:okhttp' strictly '3.10.0' because of the following reason: debugRuntimeClasspath uses version 3.10.0
							           Constraint path 'android:react-native-firebase:unspecified' --> 'com.squareup.okhttp3:okhttp' strictly '3.10.0' because of the following reason: debugRuntimeClasspath uses version 3.10.0
								           Constraint path 'android:react-native-firebase:unspecified' --> 'com.squareup.okhttp3:okhttp' strictly '3.10.0' because of the following reason: debugRuntimeClasspath uses version 3.10.0

									   > Could not resolve com.squareup.okio:okio:1.14.0.
									     Required by:
									           project :react-native-firebase
										      > Cannot find a version of 'com.squareup.okio:okio' that satisfies the version constraints:
										              Dependency path 'android:react-native-firebase:unspecified' --> 'com.facebook.react:react-native:32.0.0' --> 'com.squareup.okio:okio:1.14.0'
											              Dependency path 'android:react-native-firebase:unspecified' --> 'com.facebook.react:react-native:32.0.0' --> 'com.squareup.okhttp3:okhttp:3.12.1' --> 'com.squareup.okio:okio:1.15.0'
												              Dependency path 'android:react-native-firebase:unspecified' --> 'com.google.firebase:firebase-firestore:18.2.0' --> 'com.squareup.okhttp:okhttp:2.7.5' --> 'com.squareup.okio:okio:1.6.0'
													              Dependency path 'android:react-native-firebase:unspecified' --> 'com.google.firebase:firebase-firestore:18.2.0' --> 'io.grpc:grpc-okhttp:1.16.1' --> 'com.squareup.okio:okio:1.13.0'
														              Constraint path 'android:react-native-firebase:unspecified' --> 'com.squareup.okio:okio' strictly '1.14.0' because of the following reason: debugRuntimeClasspath uses version 1.14.0
															              Constraint path 'android:react-native-firebase:unspecified' --> 'com.squareup.okio:okio' strictly '1.14.0' because of the following reason: debugRuntimeClasspath uses version 1.14.0
																              Constraint path 'android:react-native-firebase:unspecified' --> 'com.squareup.okio:okio' strictly '1.14.0' because of the following reason: debugRuntimeClasspath uses version 1.14.0
																	              Constraint path 'android:react-native-firebase:unspecified' --> 'com.squareup.okio:okio' strictly '1.14.0' because of the following reason: debugRuntimeClasspath uses version 1.14.0

																		      > Could not resolve com.squareup.okhttp3:okhttp:3.10.0.
																		        Required by:
																			      project :react-native-firebase > com.facebook.react:react-native:32.0.0
																			            project :react-native-firebase > com.facebook.fresco:imagepipeline-okhttp3:1.10.0
																				          project :react-native-firebase > com.squareup.okhttp3:okhttp-urlconnection:3.10.0
																					     > Cannot find a version of 'com.squareup.okhttp3:okhttp' that satisfies the version constraints:
																					             Dependency path 'android:react-native-firebase:unspecified' --> 'com.facebook.react:react-native:32.0.0' --> 'com.squareup.okhttp3:okhttp:3.10.0'
																						             Dependency path 'android:react-native-firebase:unspecified' --> 'com.google.firebase:firebase-functions:16.3.0' --> 'com.squareup.okhttp3:okhttp:3.12.1'
																							             Dependency path 'android:react-native-firebase:unspecified' --> 'com.facebook.react:react-native:32.0.0' --> 'com.facebook.fresco:imagepipeline-okhttp3:1.10.0' --> 'com.squareup.okhttp3:okhttp:3.10.0'
																								             Dependency path 'android:react-native-firebase:unspecified' --> 'com.facebook.react:react-native:32.0.0' --> 'com.squareup.okhttp3:okhttp-urlconnection:3.10.0' --> 'com.squareup.okhttp3:okhttp:3.10.0'
																									             Constraint path 'android:react-native-firebase:unspecified' --> 'com.squareup.okhttp3:okhttp' strictly '3.10.0' because of the following reason: debugRuntimeClasspath uses version 3.10.0
																										             Constraint path 'android:react-native-firebase:unspecified' --> 'com.squareup.okhttp3:okhttp' strictly '3.10.0' because of the following reason: debugRuntimeClasspath uses version 3.10.0
																											             Constraint path 'android:react-native-firebase:unspecified' --> 'com.squareup.okhttp3:okhttp' strictly '3.10.0' because of the following reason: debugRuntimeClasspath uses version 3.10.0
																												             Constraint path 'android:react-native-firebase:unspecified' --> 'com.squareup.okhttp3:okhttp' strictly '3.10.0' because of the following reason: debugRuntimeClasspath uses version 3.10.0

																													     > Could not resolve com.squareup.okio:okio:1.14.0.
																													       Required by:
																													             project :react-native-firebase > com.facebook.react:react-native:32.0.0
																														        > Cannot find a version of 'com.squareup.okio:okio' that satisfies the version constraints:
																															        Dependency path 'android:react-native-firebase:unspecified' --> 'com.facebook.react:react-native:32.0.0' --> 'com.squareup.okio:okio:1.14.0'
																																        Dependency path 'android:react-native-firebase:unspecified' --> 'com.facebook.react:react-native:32.0.0' --> 'com.squareup.okhttp3:okhttp:3.12.1' --> 'com.squareup.okio:okio:1.15.0'
																																	        Dependency path 'android:react-native-firebase:unspecified' --> 'com.google.firebase:firebase-firestore:18.2.0' --> 'com.squareup.okhttp:okhttp:2.7.5' --> 'com.squareup.okio:okio:1.6.0'
																																		        Dependency path 'android:react-native-firebase:unspecified' --> 'com.google.firebase:firebase-firestore:18.2.0' --> 'io.grpc:grpc-okhttp:1.16.1' --> 'com.squareup.okio:okio:1.13.0'
																																			        Constraint path 'android:react-native-firebase:unspecified' --> 'com.squareup.okio:okio' strictly '1.14.0' because of the following reason: debugRuntimeClasspath uses version 1.14.0
																																				        Constraint path 'android:react-native-firebase:unspecified' --> 'com.squareup.okio:okio' strictly '1.14.0' because of the following reason: debugRuntimeClasspath uses version 1.14.0
																																					        Constraint path 'android:react-native-firebase:unspecified' --> 'com.squareup.okio:okio' strictly '1.14.0' because of the following reason: debugRuntimeClasspath uses version 1.14.0
																																						        Constraint path 'android:react-native-firebase:unspecified' --> 'com.squareup.okio:okio' strictly '1.14.0' because of the following reason: debugRuntimeClasspath uses version 1.14.0

																																							> Could not resolve com.squareup.okhttp3:okhttp:3.12.1.
																																							  Required by:
																																							        project :react-native-firebase > com.google.firebase:firebase-functions:16.3.0
																																								   > Cannot find a version of 'com.squareup.okhttp3:okhttp' that satisfies the version constraints:
																																								           Dependency path 'android:react-native-firebase:unspecified' --> 'com.facebook.react:react-native:32.0.0' --> 'com.squareup.okhttp3:okhttp:3.10.0'
																																									           Dependency path 'android:react-native-firebase:unspecified' --> 'com.google.firebase:firebase-functions:16.3.0' --> 'com.squareup.okhttp3:okhttp:3.12.1'
																																										           Dependency path 'android:react-native-firebase:unspecified' --> 'com.facebook.react:react-native:32.0.0' --> 'com.facebook.fresco:imagepipeline-okhttp3:1.10.0' --> 'com.squareup.okhttp3:okhttp:3.10.0'
																																											           Dependency path 'android:react-native-firebase:unspecified' --> 'com.facebook.react:react-native:32.0.0' --> 'com.squareup.okhttp3:okhttp-urlconnection:3.10.0' --> 'com.squareup.okhttp3:okhttp:3.10.0'
																																												           Constraint path 'android:react-native-firebase:unspecified' --> 'com.squareup.okhttp3:okhttp' strictly '3.10.0' because of the following reason: debugRuntimeClasspath uses version 3.10.0
																																													           Constraint path 'android:react-native-firebase:unspecified' --> 'com.squareup.okhttp3:okhttp' strictly '3.10.0' because of the following reason: debugRuntimeClasspath uses version 3.10.0
																																														           Constraint path 'android:react-native-firebase:unspecified' --> 'com.squareup.okhttp3:okhttp' strictly '3.10.0' because of the following reason: debugRuntimeClasspath uses version 3.10.0
																																															           Constraint path 'android:react-native-firebase:unspecified' --> 'com.squareup.okhttp3:okhttp' strictly '3.10.0' because of the following reason: debugRuntimeClasspath uses version 3.10.0

																																																   > Could not resolve com.squareup.okio:okio:1.15.0.
																																																     Required by:
																																																           project :react-native-firebase > com.squareup.okhttp3:okhttp:3.12.1
																																																	      > Cannot find a version of 'com.squareup.okio:okio' that satisfies the version constraints:
																																																	              Dependency path 'android:react-native-firebase:unspecified' --> 'com.facebook.react:react-native:32.0.0' --> 'com.squareup.okio:okio:1.14.0'
																																																		              Dependency path 'android:react-native-firebase:unspecified' --> 'com.facebook.react:react-native:32.0.0' --> 'com.squareup.okhttp3:okhttp:3.12.1' --> 'com.squareup.okio:okio:1.15.0'
																																																			              Dependency path 'android:react-native-firebase:unspecified' --> 'com.google.firebase:firebase-firestore:18.2.0' --> 'com.squareup.okhttp:okhttp:2.7.5' --> 'com.squareup.okio:okio:1.6.0'
																																																				              Dependency path 'android:react-native-firebase:unspecified' --> 'com.google.firebase:firebase-firestore:18.2.0' --> 'io.grpc:grpc-okhttp:1.16.1' --> 'com.squareup.okio:okio:1.13.0'
																																																					              Constraint path 'android:react-native-firebase:unspecified' --> 'com.squareup.okio:okio' strictly '1.14.0' because of the following reason: debugRuntimeClasspath uses version 1.14.0
																																																						              Constraint path 'android:react-native-firebase:unspecified' --> 'com.squareup.okio:okio' strictly '1.14.0' because of the following reason: debugRuntimeClasspath uses version 1.14.0
																																																							              Constraint path 'android:react-native-firebase:unspecified' --> 'com.squareup.okio:okio' strictly '1.14.0' because of the following reason: debugRuntimeClasspath uses version 1.14.0
																																																								              Constraint path 'android:react-native-firebase:unspecified' --> 'com.squareup.okio:okio' strictly '1.14.0' because of the following reason: debugRuntimeClasspath uses version 1.14.0

																																																									      > Could not resolve com.squareup.okio:okio:1.6.0.
																																																									        Required by:
																																																										      project :react-native-firebase > com.google.firebase:firebase-firestore:18.2.0 > com.squareup.okhttp:okhttp:2.7.5
																																																										         > Cannot find a version of 'com.squareup.okio:okio' that satisfies the version constraints:
																																																											         Dependency path 'android:react-native-firebase:unspecified' --> 'com.facebook.react:react-native:32.0.0' --> 'com.squareup.okio:okio:1.14.0'
																																																												         Dependency path 'android:react-native-firebase:unspecified' --> 'com.facebook.react:react-native:32.0.0' --> 'com.squareup.okhttp3:okhttp:3.12.1' --> 'com.squareup.okio:okio:1.15.0'
																																																													         Dependency path 'android:react-native-firebase:unspecified' --> 'com.google.firebase:firebase-firestore:18.2.0' --> 'com.squareup.okhttp:okhttp:2.7.5' --> 'com.squareup.okio:okio:1.6.0'
																																																														         Dependency path 'android:react-native-firebase:unspecified' --> 'com.google.firebase:firebase-firestore:18.2.0' --> 'io.grpc:grpc-okhttp:1.16.1' --> 'com.squareup.okio:okio:1.13.0'
																																																															         Constraint path 'android:react-native-firebase:unspecified' --> 'com.squareup.okio:okio' strictly '1.14.0' because of the following reason: debugRuntimeClasspath uses version 1.14.0
																																																																         Constraint path 'android:react-native-firebase:unspecified' --> 'com.squareup.okio:okio' strictly '1.14.0' because of the following reason: debugRuntimeClasspath uses version 1.14.0
																																																																	         Constraint path 'android:react-native-firebase:unspecified' --> 'com.squareup.okio:okio' strictly '1.14.0' because of the following reason: debugRuntimeClasspath uses version 1.14.0
																																																																		         Constraint path 'android:react-native-firebase:unspecified' --> 'com.squareup.okio:okio' strictly '1.14.0' because of the following reason: debugRuntimeClasspath uses version 1.14.0

																																																																			 > Could not resolve com.squareup.okio:okio:1.13.0.
																																																																			   Required by:
																																																																			         project :react-native-firebase > com.google.firebase:firebase-firestore:18.2.0 > io.grpc:grpc-okhttp:1.16.1
																																																																				    > Cannot find a version of 'com.squareup.okio:okio' that satisfies the version constraints:
																																																																				            Dependency path 'android:react-native-firebase:unspecified' --> 'com.facebook.react:react-native:32.0.0' --> 'com.squareup.okio:okio:1.14.0'
																																																																					            Dependency path 'android:react-native-firebase:unspecified' --> 'com.facebook.react:react-native:32.0.0' --> 'com.squareup.okhttp3:okhttp:3.12.1' --> 'com.squareup.okio:okio:1.15.0'
																																																																						            Dependency path 'android:react-native-firebase:unspecified' --> 'com.google.firebase:firebase-firestore:18.2.0' --> 'com.squareup.okhttp:okhttp:2.7.5' --> 'com.squareup.okio:okio:1.6.0'
																																																																							            Dependency path 'android:react-native-firebase:unspecified' --> 'com.google.firebase:firebase-firestore:18.2.0' --> 'io.grpc:grpc-okhttp:1.16.1' --> 'com.squareup.okio:okio:1.13.0'
																																																																								            Constraint path 'android:react-native-firebase:unspecified' --> 'com.squareup.okio:okio' strictly '1.14.0' because of the following reason: debugRuntimeClasspath uses version 1.14.0
																																																																									            Constraint path 'android:react-native-firebase:unspecified' --> 'com.squareup.okio:okio' strictly '1.14.0' because of the following reason: debugRuntimeClasspath uses version 1.14.0
																																																																										            Constraint path 'android:react-native-firebase:unspecified' --> 'com.squareup.okio:okio' strictly '1.14.0' because of the following reason: debugRuntimeClasspath uses version 1.14.0
																																																																											            Constraint path 'android:react-native-firebase:unspecified' --> 'com.squareup.okio:okio' strictly '1.14.0' because of the following reason: debugRuntimeClasspath uses version 1.14.0
																																																																												    ''''''''''''''''''''''''
																																																																								    ''''''''
																																																																							    ''''''''
																																																																						    ''''''''
																																																																					    ''''''''''''''''''''''''''''''''
																																																															 ''''''''
																																																														 ''''''''
																																																													 ''''''''
																																																												 ''''''''''''''''''''''''''''''''
																																																					      ''''''''
																																																				      ''''''''
																																																			      ''''''''
																																																		      ''''''''''''''''''''''''''''''''
																																												   ''''''''
																																											   ''''''''
																																										   ''''''
																																									   ''''''''''''''''''''''''''''''''
																																			''''''''
																																		''''''''
																																	''''''''
																																''''''''''''''''''''''''''''''''
																									     ''''''''
																								     ''''''''
																							     ''''''
																						     ''''''''''''''''''''''''''''''''
														      ''''''''
													      ''''''''
												      ''''''''
											      ''''''''''''''''''''''''''''''''
					   ''''''''
				   ''''''''
			   ''''''
		   ''''''''''
```
