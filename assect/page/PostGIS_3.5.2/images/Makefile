# **********************************************************************
# *
# * PostGIS - Spatial Types for PostgreSQL
# * http://postgis.net
# *
# * Copyright (C) 2022-2023 Sandro Santilli <strk@kbt.io>
# * Copyright 2008 Kevin Neufeld
# *
# * This is free software; you can redistribute and/or modify it under
# * the terms of the GNU General Public Licence. See the COPYING file.
# *
# **********************************************************************

PACKAGE_TARNAME = postgis

top_builddir = ../../..
top_srcdir = ../../..
srcdir = .

prefix = /usr/local
datarootdir = ${prefix}/share
docdir = /var/www/postgis_stuff
htmldir = /var/www/postgis_docs/manual-3.5

INSTALL=/usr/bin/install -c
INSTALL_DATA=${INSTALL} -m 644

CC=gcc
CFLAGS=-std=gnu11 -g -O2 -fno-math-errno -fno-signed-zeros -Wall -O2 
CPPFLAGS = -I$(top_builddir)/liblwgeom -I$(top_srcdir)/liblwgeom  -I/var/lib/jenkins/workspace/geos/rel-3.10w64/include   -I/usr/include/libxml2 -I/usr/include -I/usr/include/json-c  -DNDEBUG -I/var/lib/jenkins/workspace/pg/rel/pg13w64/include
SHELL = /bin/bash
LIBTOOL = $(SHELL) $(top_builddir)/libtool
LDFLAGS = -L/var/lib/jenkins/workspace/pg/rel/pg13w64/lib -lm -L/var/lib/jenkins/workspace/geos/rel-3.10w64/lib -lgeos_c -lproj



STATIC_IMAGES_SRC = $(wildcard $(srcdir)/static/*.png $(srcdir)/static/*.gif)
STATIC_IMAGES = $(subst $(srcdir)/static/,,$(STATIC_IMAGES_SRC))

GENERATED_IMAGES= \
  cg_approxconvexpartition01.png \
	cg_greeneapproxconvexpartition01.png \
	cg_optimalconvexpartition01.png \
  cg_visibility01.png \
	cg_visibility02.png \
	cg_visibility03.png \
	cg_ymonotonepartition01.png \
	cg_ymonotonepartition02.png \
	de9im01.png \
	de9im02.png \
	st_alphashape01.png \
	st_alphashape02.png \
	st_alphashape03.png \
	st_azimuth01.png \
	st_azimuth02.png \
	st_boundary01.png \
	st_boundary02.png \
	st_buffer01.png \
	st_buffer02.png \
	st_buffer03.png \
	st_buffer04.png \
	st_buffer05.png \
	st_buffer06.png \
	st_buffer07.png \
	st_buffer08.png \
	st_buffer09.png \
	st_buffer10.png \
	st_buffer11.png \
	st_buffer12.png \
	st_buffer13.png \
	st_buildarea01.png \
	st_buildarea02.png \
	st_buildarea03.png \
	st_closestpoint01.png \
	st_closestpoint02.png \
	st_clusterkmeans02.png \
	st_centroid01.png \
	st_centroid02.png \
	st_centroid03.png \
	st_centroid04.png \
	st_chaikinsmoothing01.png \
	st_chaikinsmoothing02.png \
	st_chaikinsmoothing03.png \
	st_chaikinsmoothing04.png \
	st_chaikinsmoothing05.png \
	st_chaikinsmoothing06.png \
	st_contains01.png \
	st_contains02.png \
	st_contains03.png \
	st_contains04.png \
	st_contains05.png \
	st_contains06.png \
	st_contains07.png \
	st_contains08.png \
	st_concavehull01.png \
	st_concavehull02.png \
	st_concavehull03.png \
	st_concavehull04.png \
	st_convexhull01.png \
	st_coverageinvalidedges01.png \
	st_coveragesimplify01.png \
	st_coveragesimplify02.png \
	st_coverageunion01.png \
	st_coverageunion02.png \
	st_crosses01.png \
	st_crosses02.png \
	st_crosses03.png \
	st_crosses04.png \
	st_constraineddelaunaytriangles01.png \
	st_constraineddelaunaytriangles02.png \
	st_delaunaytriangles04.png \
	st_difference01.png \
	st_dumppoints01.png \
	st_envelope01.png \
	st_extrude01.png \
	st_extrude03.png \
	st_generatepoints01.png \
	st_geometricmedian01.png \
	st_hausdorffdistance01.png \
	st_issimple01.png \
	st_issimple02.png \
	st_issimple03.png \
	st_issimple04.png \
	st_issimple05.png \
	st_issimple06.png \
	st_issimple07.png \
	st_isvalid01.png \
	st_isvalid02.png \
	st_isvalid03.png \
	st_isvalid04.png \
	st_isvalid05.png \
	st_isvalid06.png \
	st_isvalid07.png \
	st_isvalid08.png \
	st_isvalid09.png \
	st_largestemptycircle01.png \
	st_largestemptycircle02.png \
	st_letters01.png \
	st_linecrossingdirection01.png \
	st_linecrossingdirection02.png \
	st_linecrossingdirection03.png \
	st_linecrossingdirection04.png \
	st_line_interpolate_point01.png \
	st_line_interpolate_points01.png \
	st_linemerge01.png \
	st_linemerge02.png \
	st_linemerge03.png \
	st_line_substring01.png \
	st_locatebetween01.png \
	st_longestline01.png \
	st_longestline02.png \
	st_longestline03.png \
	st_makevalid01.png \
	st_makevalid02.png \
	st_makevalid03.png \
	st_makevalid04.png \
	st_makevalid05.png \
	st_makevalid06.png \
	st_maximuminscribedcircle01.png \
	st_maximuminscribedcircle02.png \
	st_minimumboundingcircle01.png \
	st_minkowskisum01.png \
	st_minkowskisum02.png \
	st_minkowskisum03.png \
	st_minkowskisum04.png \
	st_offsetcurve01.png \
	st_offsetcurve02.png \
	st_offsetcurve03.png \
	st_offsetcurve04.png \
	st_offsetcurve05.png \
	st_offsetcurve06.png \
	st_optimalalphashape01.png \
	st_optimalalphashape02.png \
	st_orientedenvelope01.png \
	st_overlaps01.png \
	st_overlaps02.png \
	st_overlaps03.png \
	st_overlaps04.png \
	st_overlaps05.png \
	st_overlaps06.png \
	st_pointonsurface.png \
	st_pointonsurface01.png \
	st_pointonsurface02.png \
	st_pointonsurface03.png \
	st_pointonsurface04.png \
	st_polygonize01.png \
	st_polygonize02.png \
	st_triangulatepolygon01.png \
	st_triangulatepolygon02.png \
	st_segmentize01.png \
	st_sharedpaths01.png \
	st_sharedpaths02.png \
	st_shortestline01.png \
	st_shortestline02.png \
	st_snap01.png \
	st_snap02.png \
	st_snap03.png \
	st_snap04.png \
	st_snap05.png \
	st_split01.png \
	st_split02.png \
	st_split03.png \
	st_split04.png \
	st_simplify01.png \
	st_simplify02.png \
	st_simplifypolygonhull01.png \
	st_simplifypolygonhull02.png \
	st_simplifypolygonhull03.png \
	st_simplifypreservetopology01.png \
	st_simplifypreservetopology02.png \
	st_simplifyvw01.png \
	st_simplifyvw02.png \
	st_straightskeleton01.png \
	st_approximatemedialaxis01.png \
	st_subdivide01.png \
	st_subdivide02.png \
	st_symdifference01.png \
	st_symdifference02.png \
	st_tesselate03.png \
	st_tesselate04.png \
	st_touches01.png \
	st_touches02.png \
	st_touches03.png \
	st_touches04.png \
	st_touches05.png \
	st_touches06.png \
	st_voronoi01.png \
	st_voronoi02.png \
	st_voronoi03.png \
	st_within01.png

# Images that are created with dimensions 100x100
GENERATED_IMAGES_RESIZED= \
	de9im03.png \
	de9im04.png \
	de9im05.png \
	de9im06.png \
	de9im07.png \
	de9im08.png \
	de9im09.png \
	de9im10.png \
	de9im11.png \
	de9im12.png \
	de9im13.png

ALL_IMAGES = \
	$(GENERATED_IMAGES) \
	$(GENERATED_IMAGES_RESIZED) \
	$(STATIC_IMAGES)

OBJS=styles.o generator.o

# Build the generator
all: generator

# generate the images
images: $(ALL_IMAGES)

images-install: $(ALL_IMAGES)
	mkdir -p $(DESTDIR)$(htmldir)/images
	$(INSTALL_DATA) $(ALL_IMAGES) $(DESTDIR)$(htmldir)/images/

images-uninstall:
	rm -f $(ALL_IMAGES:%=$(DESTDIR)$(htmldir)/images/%)

# Command to build each of the .o files
$(OBJS): %.o: %.c
	$(CC) $(CPPFLAGS) $(CFLAGS) -c -o $@ $<

# Command to symlink each of the static images
$(STATIC_IMAGES):
	ln -fs $(srcdir)/static/$@ $@

# Command to build each of the .wkt files
$(GENERATED_IMAGES): %.png: wkt/%.wkt generator wkt/styles.conf
	@./generator $< $@

# Command to resize each of the images
$(GENERATED_IMAGES_RESIZED): %.png: wkt/%.wkt generator wkt/styles.conf
	./generator -s 100x100 $< $@

# Build the main executable
generator: $(OBJS) ../../../liblwgeom/.libs/liblwgeom.a
	$(LIBTOOL) --mode=link \
	$(CC) -o $@ $^ $(LDFLAGS)

# Build liblwgeom
../../../liblwgeom/.libs/liblwgeom.a:
	$(MAKE) -C ../../../liblwgeom liblwgeom.la

# Clean target
clean:
	rm -f $(OBJS)
	rm -f generator
	rm -rf generator-temp-*

distclean: clean
	rm -f Makefile

images-clean:
	rm -f $(ALL_IMAGES)

.NOTPARALLEL:
